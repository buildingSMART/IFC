The standard wall (_IfcWallStandardCase_) defines a wall with certain constraints for the provision of parameters and with certain constraints for the geometric representation. The _IfcWallStandardCase_ handles all cases of walls, that are extruded vertically&nbsp;

* along the positive z axis of the wall local placement coordinate system, and
* along the positive z axis of the global (world) coordinate system

and have a single thickness along the path, i.e.:

* parallel sides for straight walls
* co-centric sides for curved walls.

The following parameter shall be given:

* Wall height, taken from the depth of extrusion, provided by the geometric representation.
* Wall thickness, taken from the material layer set usage, attached to the wall
* Wall offset from axis, taken from the material layer set usage, attached to the wall

The material of the wall is defined by the _IfcMaterialLayerSetUsage_ and is attached by the _IfcRelAssociatesMaterial_ objectified relationship. It is accessible by the inverse _HasAssociations_ relationship. The material layer set usage has to be given (enforced by where rule).

> <small><font color="#0000ff">HISTORY New entity in IFC Release 2x.</font></small>

****Type Use Definition****

The type information relating to the _IfcWallStandardCase_ is defined at the supertype _IfcWall_. As an additional use agreement for standard walls, the _IfcWallType_ should have a unique _IfcMaterialLayerSet_, that is referenced by the&nbsp;_IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcWallType_.

<table border="0" cellpadding="2" cellspacing="2" width="100%"><tbody><tr><td><p><img alt="Material layer set and usage" src="figures/ifcwallstandardcase_materialusage-01.png" height="220" width="501">&nbsp;</p></td><td align="left" valign="top"><small>Assignment of <i>IfcMaterialLayerSetUsage</i>
and <i>IfcMaterialLayerSet</i> to the wall type and the
wall occurrence.</small></td></tr></tbody></table>

****Property
Set Use Definition****:

The property sets relating to the _IfcWallStandardCase_ are defined at the supertype _IfcWall_.

****Quantity
Use Definition****:

The quantities relating to the _IfcWallStandardCase_ are defined at the supertype _IfcWall_.

****Geometry
Use Definitions****:

The geometric representation of _IfcWallStandardCase_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation. Included are:

**Local
Placement**

The use of local placement is defined at the supertype _IfcWall_.

**_Geometric
Representation_**

The standard geometric representation of _IfcWallStandardCase_ is defined using the following multiple shape representations for its definition:

* **Axis**: A two-dimensional open curve (_IfcBoundedCurve_) defining the axis for the standard wall. The material layer offset is measured from the wall axis.
* **Body**: A Swept Solid Representation or a CSG representation defining the 3D shape of the standard wall

**First
representation: Curve2D representation of wall axis**

The wall axis is represented by a two-dimensional open curve within a particular shape representation. The wall axis is used to apply the parameter to the wall geometry. The following attribute values shall be used

> _IfcShapeRepresentation_ shall have the following values:
> 
> * RepresentationIdentifier : 'Axis'
> * RepresentationType : 'Curve2D'

<table cellpadding="2" cellspacing="2">
<tbody> <tr> <td align="left" valign="top"><a href="drawings/IfcWallStandard_StraigthWall_01-Layout1.dwf"><img src="figures/ifcwallstandard_straigthwall_01-layout1.gif" alt="straight wall axis" border="0" height="299" width="393"></a></td> <td align="left" valign="top"> <p><font size="-1">In case
of a straight wall, the set of items shall include a single geometric
representation item of type <i>IfcPolyline</i> or <i>IfcTrimmedCurve</i>
with the <i>BasisCurve</i> being an <i>IfcLine</i>.</font></p>
</td> </tr> <tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcWallStandard_CurvedWall_01-Layout1.dwf"><img src="figures/ifcwallstandard_curvedwall_01-layout1.gif" alt="curved wall axis" border="0" height="299" width="393"></a></td> <td align="left" valign="top"> <p><font size="-1">In case
of a curved wall, the set of items shall include a single geometric
representation item of type <i>IfcTrimmedCurve</i>. The
curve shall have a <i>BasisCurve</i> of type <i>IfcCircle</i>.</font></p>
</td> </tr> </tbody></table>

**Second
representation: SweptSolid or
Clipping representation of wall body**

The body of the _IfcWallStandardCase_ is defined by using 'SweptSolid' representation for walls without clippings or 'Clipping' representation for walls with clippings (e.g. under sloped roof slabs).

> _IfcShapeRepresentation_ shall have the following values:
> 
> * RepresentationIdentifier : 'Body'
> * RepresentationType : 'SweptSolid' or 'Clipping'

**SweptSolid representation**

The standard geometric representation (for body) of _IfcWallStandardCase_ is defined using the 'SweptSolid' representation. The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ and _IfcRectangleProfileDef_ shall be supported. 
* **Extrusion**: The profile shall be extruded vertically, i.e., in the direction of the z-axis of the co-ordinate system of the referred spatial structure element. It might be further constraint to be in the direction of the global z-axis in implementers agreements. The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the Position of the _IfcExtrudedAreaSolid_.

<table cellpadding="2" cellspacing="2"> <tbody><tr>
<td align="left" valign="top"><a href="drawings/IfcWallStandard_StraigthWall_02-Layout1.dwf"><img src="figures/ifcwallstandard_straigthwall_02-layout1.gif" alt="straight wall body" border="0" height="299" width="393"></a></td> <td align="left" valign="top"> <p><font size="-1">The
profile of a wall is described in the ground view and extruded
vertically. The profile (also identical with the foot print of the
wall) is defined by the <i>IfcArbitraryClosedProfileDef</i>
(excluding its subtypes). The profile is given with all wall
connections already resolved. </font></p> <ul> <li><font size="-1">In case of a straight wall the two sides of the
profile shall be parallel to the wall axis, i.e. the wall has a single
unchanged thickness.</font></li> </ul> </td> </tr>
<tr> <td align="left" valign="top"><a href="drawings/IfcWallStandard_CurvedWall_02-Layout1.dwf"><img src="figures/ifcwallstandard_curvedwall_02-layout1.gif" alt="curved wall body" border="0" height="299" width="393"></a></td> <td align="left" valign="top"> <ul> <li><font size="-1">In
case of a curved wall the two sides of the profile shall be parallel
(with defined offset) to the wall axis, i.e. the wall has a single
unchanged thickness.</font></li> </ul> </td> </tr>
</tbody></table>

The advanced geometric representation (for body) of _IfcWallStandardCase_ is defined using the 'Clipping' representation. The following additional constraints apply to the swept solid representation:

* **Solid**: see standard geometric representation
* **Profile**: see standard geometric representation 
* **Extrusion**: see standard geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or subtypes). 

<table cellpadding="2" cellspacing="2"><tbody>
<tr> <td><a href="drawings/IfcWallStandard_StraigthWall_03-Layout1.dwf"><img src="figures/ifcwallstandard_straigthwall_03-layout1.gif" alt="straight wall clipping" border="0" height="299" width="397"></a></td> <td align="left" valign="top"> <p><font size="-1">Example
of clipping using an <i>IfcPolygonalBoundedHalfSpace</i>
as <i>SecondOperand</i> in the <i>IfcBooleanClippingResult</i>.</font></p>
</td> </tr> <tr> <td><a href="drawings/IfcWallStandard_CurvedWall_03-Layout1.dwf"><img src="figures/ifcwallstandard_curvedwall_03-layout1.gif" alt="curved wall clipping" border="0" height="300" width="400"></a></td> <td align="left" valign="top"> <p><font size="-1">Example
of clipping using an <i>IfcHalfSpaceSolid</i> as <i>SecondOperand</i>
in the <i>IfcBooleanClippingResult</i>.</font></p>
</td> </tr> </tbody></table>