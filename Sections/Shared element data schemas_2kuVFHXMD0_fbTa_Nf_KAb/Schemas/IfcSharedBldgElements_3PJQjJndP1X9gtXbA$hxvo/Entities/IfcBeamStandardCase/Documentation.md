The standard beam, _IfcBeamStandardCase_, defines a beam with certain constraints for the provision of material usage, parameters and with certain constraints for the geometric representation. The _IfcBeamStandardCase_ handles all cases of beams, that:

* have a reference to the _IfcMaterialProfileSetUsage_ defining the material profile association of the beam with the cardinal point of its insertion relative to the local placement.
* are consistent in using the correct cardinal point offset of the profile as compared to the 'Axis' and 'Body' shape representation
* are based on a sweep of a planar profile, or set of profiles, as defined by the _IfcMaterialProfileSet_
* have an 'Axis' shape representation with constraints provided below in the geometry use definition
* have a 'Body' shape representation with constraints provided below in the geometry use definition 
    * are extruded perpendicular to the profile definition plane
    * have a start profile, or set of profiles, that is swept
    * the sweeping operation can be linear extrusion, circular rotation, or a sweep along a directrix
    * the start profile, or set of profiles can be swept unchanged, or might be changed uniformly by a taper definition 
*  
>> NOTE&nbsp; View definitions and implementer agreements may further constrain the applicable geometry types, e.g. by excluding tapering from an _IfcBeamStandardCase_ implementation. 

> HISTORY&nbsp; New entity in IFC4.

**_Geometric Representations_**

The geometric representation of _IfcBeamStandardCase_ is defined using the following multiple shape representations for its definition:

* **Axis**: A three dimensional open curve (subtype of _IfcBoundedCurve_) defining the axis for the standard beam. The cardinal point is determined by the beam axis.
* **Body**: A Swept Solid Representation or a CSG clipping representation defining the 3D shape of the standard beam.

> NOTE&nbsp; It is invalid to exchange a 'SurfaceModel', 'Brep', or 'MappedRepresentation' representation for the 'Body' shape representation of an _IfcBeamStandardCase_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcBuildingElement_: [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)
* _IfcBeam_: [Object Typing](../../templates/object-typing.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Quantity Sets](../../templates/quantity-sets.htm), [Spatial Containment](../../templates/spatial-containment.htm), [Element Composition](../../templates/element-composition.htm), [Material Profile Set](../../templates/material-profile-set.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcbeamstandardcase.htm)

{ .use-head}
Material Profile Set Usage

The [Material Profile Set Usage](../../templates/material-profile-set-usage.htm) concept applies to this entity.

The _IfcBeamStandardCase_ defines in addition that the _IfcBeamType_ should have a unique _IfcMaterialProfileSet_, that is referenced by the _IfcMaterialProfileSetUsage_ that is assigned to all occurrences of this _IfcBeamType_.

<table>

 <tr>
  <td><img src="../../../figures/IfcBeamStandardCase-01.png" height="500" width="500" alt="Material profile set and usage"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialProfileSetUsage</em> and <em>IfcMaterialProfileSet</em> to the <em>IfcBeamStandardCase</em> as the beam occurrence and to the <em>IfcBeamType</em>. The same <em>IfcMaterialProfileSet</em> shall be shared by many occurrences of <em>IfcMaterialProfileSetUsage</em>. This relationship shall be consistent to the relationship between the <em>IfcBeamType</em> and the <em>IfcBeamStandardCase</em>.</blockquote>

 </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Beam profile usage</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table>

 <tr>
  <td><img src="../../../figures/IfcBeamStandardCase_CardinalPoint.png" height="250" width="500" alt="Cardinal point usage"></td>
  <td>

    <blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates alignment of cardinal points.</blockquote>
    
<blockquote class="note">NOTE&nbsp; It has to be guaranteed that the use of <em>IfcCardinalPointEnum</em> is consistent to the placement of the extrusion body provided by <em>IfcExtrudedAreaSolid.Position</em></blockquote>
    
<blockquote class="note">NOTE&nbsp; The cardinal points <b>8</b> (top centre) and <b>6</b> (mid-depth right) are assigned according to the definition at <em>IfcCardinalPointReference</em></blockquote> </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 2 &mdash; Beam cardinal points</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table>
 
<tr>
  <td><img src="../../../figures/IfcBeamStandardCase-02.png" height="550" width="500" alt="Material profile set and usage"></td>
  <td>
<blockquote class="example">EXAMPLE&nbsp; Figure 3 illustrates assignment of a composite profile by using <em>IfcCompositeProfile</em> for geometric representation and several <em>IfcMaterialProfile</em>'s within the <em>IfcMaterialProfileSet</em>.</blockquote>

 </td>
 </tr>

 <tr>
  <td><p class="figure">Figure 3 &mdash; Beam composite profiles</p></td>
 </tr>

</table>

  
  
{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Relative</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>Relative placement according to position and rotation relative to container.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>&nbsp;</td><td>Absolute placement according to position and rotation of world coordinate system.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifcgridplacement.htm">IfcGridPlacement</a></td><td>&nbsp;</td><td>Placement according to grid intersection.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcBeamStandardCase Product Placement</p></td></tr></table>

The following restriction is imposed:

* The local placement shall provide the location and directions for the standard beam, the x/y plane is the plane for the start profile, and the z-axis is the extrusion axis for the beam body (in case of rotation, the tangent direction).

  
  
{ .use-head}
Axis 3D Geometry

The [Axis 3D Geometry](../../templates/axis-3d-geometry.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>Axis</td><td>Curve3D</td><td><a href="../../ifcgeometryresource/lexical/ifcboundedcurve.htm">IfcBoundedCurve</a></td><td>Three-dimensional reference curve for the beam.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcBeamStandardCase Axis 3D Geometry</p></td></tr></table>

The following additional constraints apply to the 'Axis' representation, if the 'Body' shape representation has the _RepresentationType_ : 'SweptSolid':

* _Axis_ 
    * _IfcPolyline_ having two _Points_, or _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcLine_ for 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the z axis of the object coordinate system.
    * _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcCircle_ for 'SweptSolid' provided as _IfcRevolvedAreaSolid_. The axis curve lies on the x/z plane of the object coordinate system, the tangent at the start is along the positive z-axis. 

&nbsp;

<table border="0" cellpadding="2" cellspacing="2" summary="Axis">

<tr><td align="left" valign="top" width="350">
<img src="../../../figures/IfcBeamStandardCase_Axis-01.png" alt="Axis" height="300" width="400" border="1"></td>
<td><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 76, the axis shall be defined along the z axis of the object coordinate system. The axis representation can be used to represent the system length of a beam that may extent the body length of the beam.</blockquote>

</td>
</tr>

<tr><td><p class="figure">Figure 4 &mdash; Beam axis representation</p></td><td>&nbsp;</td></tr>

</table>

<table>

<tr><td align="left" valign="top" width="350">
<img src="../../../figures/IfcBeamStandardCase_Axis-02.png" alt="Axis" height="300" width="400" border="1"></td>
<td><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 77, the axis representation shall be used to represent the cardinal point as the offset between the 'Axis' and the extrusion path of the beam. The extrusion path is provided as <em>IfcExtrudedAreaSolid.ExtrudedDirection</em> and should be parallel to the 'Axis' and the z axis. It has to be guaranteed that the value provided by
<em>IfcMaterialProfileSetUsage.CardinalPoint</em> is consistent to the <em>IfcExtrudedAreaSolid.Position</em>.</blockquote>

</td>
</tr>

<tr><td><p class="figure">Figure 5 &mdash; Beam axis cardinal point</p></td><td>&nbsp;</td></tr>

</table>

  
  
{ .use-head}
Body SweptSolid Geometry

The [Body SweptSolid Geometry](../../templates/body-sweptsolid-geometry.htm) concept applies to this entity.

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Solid Position** : The _IfcSweptAreaSolid.Position_ shall exclusively been used to correspond to the cardinal point. The x/y offset of the _Position_ represents the cardinal point offset of the profile against the axis. No rotation shall be allowed.
* **Profile**: All subtypes of _IfcParameterizedProfileDef_
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.
* **Extrusion**:&nbsp;Perpendicular to the profile direction. The _IfcExtrudedAreaSolid.ExtrudedDirection_ shall be [0.,0.,1.].
* **Orientation**: The y-axis of the profile, as determined by _IfcSweptAreaSolid.Position.P[2]_ shall point upwards. It indicates the "role" of the beam, a role=0&deg; means y-axis of profile pointing upwards.

Figure 6 illustrates a standard geometric representation with cardinal point applied as **1** (bottom left).

The following interpretation of dimension parameter applies for rectangular beams with linear extrusions:

* _IfcRectangleProfileDef.YDim_ interpreted as beam height
* _IfcRectangleProfileDef.XDim_ interpreted as beam width

The following interpretation of dimension parameter applies for circular beams:

* _IfcCircleProfileDef.Radius_ interpreted as beam radius.

!["standard beam"](../../../figures/IfcBeamStandardCase_SweptSolid-01.png "Figure 6 &mdash; Beam body extrusion")

  
  
{ .use-head}
Body AdvancedSweptSolid Geometry

The [Body AdvancedSweptSolid Geometry](../../templates/body-advancedsweptsolid-geometry.htm) concept applies to this entity.

The following additional constraints apply to the 'AdvancedSweptSolid' representation type:

* **Solid**: _IfcSurfaceCurveSweptAreaSolid_, _IfcFixedReferenceSweptAreaSolid_, _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported. 
>> NOTE&nbsp; View definitions and implementer agreement can further constrain the allowed swept solid types. 
* **Solid Position** : see 'SweptSolid' geometric representation
* **Profile**: see 'SweptSolid' geometric representation
* **Profile Position** : see 'SweptSolid' geometric representation
* **Extrusion**:&nbsp;not applicable

  
  
{ .use-head}
Body Clipping Geometry

The [Body Clipping Geometry](../../templates/body-clipping-geometry.htm) concept applies to this entity.

The following constraints apply to the 'Clipping' representation:

* **Solid** : see 'SweptSolid' geometric representation
* **Solid Position** : see 'SweptSolid' geometric representation
* **Profile** : see 'SweptSolid' geometric representation
* **Profile Position** : see 'SweptSolid' geometric representation
* **Extrusion** : see 'SweptSolid' geometric representation
* **Orientation** : see 'SweptSolid' geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or its subtypes).

Figure 7 illustrates a 'Clipping' geometric representation with use of _IfcBooleanClippingResult_ between an _IfcExtrudedAreaSolid_ and an _IfcHalfSpaceSolid_ to create a clipped body, with cardinal point applied as **4** (mid-depth left)

!["clipped beam"](../../../figures/IfcBeamStandardCase_Clipping-01.png "Figure 7 &mdash; Beam body clipping")