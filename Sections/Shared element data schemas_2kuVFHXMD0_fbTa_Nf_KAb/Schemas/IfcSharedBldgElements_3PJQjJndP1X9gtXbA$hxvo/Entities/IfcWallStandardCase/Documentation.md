The _IfcWallStandardCase_ defines a wall with certain constraints for the provision of parameters and with certain constraints for the geometric representation. The _IfcWallStandardCase_ handles all cases of walls, that are extruded vertically:

* along the positive z axis of the wall object coordinate system, and
* along the positve z axis of the global (world) coordinate system

and have a single thickness along the path for each wall layer, i.e.:

* parallel sides for straight walls
* co-centric sides for curved walls.

and have either:

* a straight line axis (straight wall), or
* a circular arc axis (round wall).

and shall not have

* aggregated components, that is, parts aggregated to a wall by _IfcRelAggregates_
* shape representation for 'Body' not being an extrusion, or clipped extrusion

The following parameter have to be provided:

* Wall height, taken from the depth of extrusion, provided by the geometric representation.
* Wall thickness, taken from the material layer set usage, attached to the wall
* Wall offset from axis, taken from the material layer set usage, attached to the wall

The _IfcWallStandardCase_ requires the provision of the wall axis either a straight line that is parallel to the x-axis of the object coordinate system, or a circular arc where the tangent at start is parallel to the x-axis of the object coordinate system. The direction of the wall axis shall be the positive direction of that x-axis.

The material of the wall is defined by the _IfcMaterialLayerSetUsage_ and is attached by the _IfcRelAssociatesMaterial_ objectified relationship. It is accessible by the inverse _HasAssociations_ relationship. The material layer set usage has to be given (enforced by where rule).

> HISTORY&nbsp; New entity in IFC2x.

The standard geometric representation of _IfcWallStandardCase_ is defined using the following multiple shape representations for its definition:

* **Axis**: A two-dimensional open curve (_IfcBoundedCurve_) defining the axis for the standard wall. The material layer offset is measured from the wall axis.
* **Body**: A Swept Solid Representation or a CSG representation defining the 3D shape of the standard wall

> NOTE&nbsp; It is invalid to exhange a 'SurfaceModel', or 'Brep' or 'MappedRepresentation' representation for the 'Body' shape representation of an _IfcWallStandardCase_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcBuildingElement_: [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)
* _IfcWall_: [Object Typing](../../templates/object-typing.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Quantity Sets](../../templates/quantity-sets.htm), [Material Layer Set](../../templates/material-layer-set.htm), [Path Connectivity](../../templates/path-connectivity.htm), [Spatial Containment](../../templates/spatial-containment.htm), [Surface Geometry](../../templates/surface-geometry.htm), [Element Voiding](../../templates/element-voiding.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcwallstandardcase.htm)

{ .use-head}
Material Layer Set Usage

The [Material Layer Set Usage](../../templates/material-layer-set-usage.htm) concept applies to this entity.

Multi-layer walls can be represented by refering to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_ that is referenced from the _IfcMaterialLayerSetUsage_.&nbsp;

Material information can also be given at the _IfcWallType_, defining the common attribute data for all occurrences of the same type. It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _IfcSlabType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_.

The _IfcWallType_ should then have a unique _IfcMaterialLayerSet_, that is referenced by the _IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcWallType_.

&nbsp;

<table>
 
<tr>
  <td><img src="../../../figures/IfcWallStandardCase_MaterialUsage-01.png" alt="Material layer set and usage" height="220" width="501"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialLayerSetUsage</em> and <em>IfcMaterialLayerSet</em> to the wall type and the wall occurrence.</blockquote></td>
 </tr>

 <tr>
  <td><p class="figure">Figure 1 &mdash; Wall Standard Object Typing</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

Figure 2 illustrates material layer usage, where the following conventions shall be met:

* The reference coordinate system is the local coordinate system established by the _ObjectPlacement_ of the _IfcWallStandardCase_.
* The reference axis is the axis defined by the _IfcShapeRepresentation_ with _RepresentationType_='Axis' as one of the _Representation.Representations_ of the _IfcWallStandardCase_.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is given as a distance from this axis.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is the distance parallel to the reference axis and always within the base (XY) plane of the reference coordinate system. A positve value of _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ would then point into the positive y-axis of the reference coordinate system.
* The _IfcMaterialLayerSetUsage.DirectionSense_ defines how the _IfcMaterialLayer_'s are assigned to the reference axis. POSITIVE means in direction to the positive y-axis of the reference coordinate system.
* The _Thickness_ of each _IfcMaterialLayer_ is provided starting from the _OffsetFromReferenceLine_ and in the direction given by _DirectionSense_. It is applied without any gap or overlap between two consecutive layers. The _TotalThickness_ of the _IfcMaterialLayerSet_ is the sum of all layer thicknesses.
* The _IfcMaterialLayerSetUsage.LayerSetDirection_ is always AXIS2.

!["roof slab material layer set"](../../../figures/IfcMaterialLayerSetUsage_Wall-01.png "Figure 2 &mdash; Wall material layers")

  
  
{ .use-head}
Axis 2D Geometry

The [Axis 2D Geometry](../../templates/axis-2d-geometry.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>Axis</td><td>Curve2D</td><td><a href="../../ifcgeometryresource/lexical/ifcboundedcurve.htm">IfcBoundedCurve</a></td><td>The wall axis of the wall.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcWallStandardCase Axis 2D Geometry</p></td></tr></table>

The wall axis is represented by a two-dimensional open curve within a particular shape representation. The wall axis is used to apply the material layer set usage parameter to the wall geometry.

* _Axis_ 
    * _IfcPolyline_ having two _Points_, or _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcLine_ for the 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the x/y plane and is parallel to the x-axis of the object coordinate system.
    * _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcCircle_ for 'SweptSolid' provided as _IfcRevolvedAreaSolid_. The axis curve lies on the x/y plane of the object coordinate system, the tangent at the start is along the positive x-axis. 

&nbsp;

<table cellpadding="2" cellspacing="2">

 <tr>

  <td align="left" valign="top"><img src="../../../figures/IfcWallStandard_StraigthWall_01-Layout1.gif" alt="straight wall axis" border="0" height="299" width="393"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 3 illustrates an axis representation for a straight wall. In case of a straight wall, the set of items shall
include a single geometric representation item of type <em>IfcPolyline</em> or <em>IfcTrimmedCurve</em> with the <em>BasisCurve</em> being an <em>IfcLine</em>. The <em>IfcPolyline</em> or <em>IfcTrimmedCurve</em> shall be parallel (here in a special case co-linear) to the x-axis
of the object coordinate system. The direction shall be identical to the direction of the x-axis.</blockquote>

 </td>
 </tr>
 <tr>
  <td width="393"><p class="figure">Figure 3 &mdash; Wall axis straight</p></td>

  <td>&nbsp;</td>
 </tr>
</table>

<table cellpadding="2" cellspacing="2">

 <tr>

  <td align="left" valign="top"><img src="../../../figures/IfcWallStandard_CurvedWall_01-Layout1.gif" alt="curved wall axis" border="0" height="299" width="393"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 4 illustrates an axis representation for a curved wall. In case of a curved wall, the set of items shall include
a single geometric representation item of type <em>IfcTrimmedCurve</em>. The curve shall have a <em>BasisCurve</em> of type <em>IfcCircle</em>. The tangent of the <em>IfcTrimmedCurve</em> shall be parallel at start to the x-axis of the object coordinate system. The direction shall be identical to the direction of the x-axis.</blockquote>
 </td></tr>
 
<tr>
  <td width="393"><p class="figure">Figure 4 &mdash; Wall axis curved</p></td>
  <td>&nbsp;</td>
 
</tr>

</table>

  
  
{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Relative</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>Relative placement according to position and rotation relative to container.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>&nbsp;</td><td>Absolute placement according to position and rotation of world coordinate system.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifcgridplacement.htm">IfcGridPlacement</a></td><td>&nbsp;</td><td>Placement according to grid intersection.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcWallStandardCase Product Placement</p></td></tr></table>

The following restriction is imposed:

* The local placement shall provide the location and directions for the standard wall, the x/y plane is the plane for the profile, and the z-axis is the extrusion axis for the wall body.

  
  
{ .use-head}
Body SweptSolid Geometry

The [Body SweptSolid Geometry](../../templates/body-sweptsolid-geometry.htm) concept applies to this entity.

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ and _IfcRectangleProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded vertically, i.e., in the direction of the z-axis of the co-ordinate system of the referred spatial structure element. It might be further constraint to be in the direction of the global z-axis in implementers agreements. The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the Position of the _IfcExtrudedAreaSolid_.

The profile of a wall is described in the ground view and extruded vertically. The profile (also identical with the foot print of the wall) is defined by the _IfcArbitraryClosedProfileDef_ (excluding its subtypes). The profile is given with all wall connections already resolved.

Figure 5 illustrates a body representation for a straight wall. In case of a straight wall, the two sides of the profile shall be parallel to the wall axis, that is, the wall has a single unchanged thickness.

Figure 6 illustrates a body representation for a curved wall. In case of a curved wall, the two sides of the profile shall be parallel (with defined offset) to the wall axis, that is, the wall has a single unchanged thickness.

<table cellpadding="2" cellspacing="2">
<tr>
<td align="left" valign="top"><img src="../../../figures/IfcWallStandard_StraigthWall_02-Layout1.gif" alt="straight wall body" border="0" height="299" width="393"></td>
<td align="left" valign="top"><img src="../../../figures/IfcWallStandard_CurvedWall_02-Layout1.gif" alt="curved wall body" border="0" height="299" width="393"></td>
</tr>
<tr>
<td width="393"><p class="figure">Figure 5 &mdash; Wall body extrusion straight</p></td>
<td width="393"><p class="figure">Figure 6 &mdash; Wall body extrusion curved</p></td>
</tr>
</table>

  
  
{ .use-head}
Body Clipping Geometry

The [Body Clipping Geometry](../../templates/body-clipping-geometry.htm) concept applies to this entity.

The following constraints apply to the 'Clipping' representation:

* **Solid**: see standard geometric representation
* **Profile**: see standard geometric representation
* **Extrusion**: see standard geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or subtypes).

Figure 7 illustrates a clipping for a straight wall using an _IfcPolygonalBoundedHalfSpace_ as _SecondOperand_ in the _IfcBooleanClippingResult_.

Figure 8 illustrates a clipping for a curved wall using an _IfcHalfSpaceSolid_ as _SecondOperand_ in the _IfcBooleanClippingResult_.

<table cellpadding="2" cellspacing="2">
<tr>
<td><img src="../../../figures/IfcWallStandard_StraigthWall_03-Layout1.gif" alt="straight wall clipping" border="0" height="299" width="397"></td>
<td><img src="../../../figures/IfcWallStandard_CurvedWall_03-Layout1.gif" alt="curved wall clipping" border="0" height="300" width="400"></td>
</tr>
<tr>
<td width="397"><p class="figure">Figure 7 &mdash; Wall body clipping straight</p></td>
<td width="400"><p class="figure">Figure 8 &mdash; Wall body clipping curved</p></td>
</tr>
</table>