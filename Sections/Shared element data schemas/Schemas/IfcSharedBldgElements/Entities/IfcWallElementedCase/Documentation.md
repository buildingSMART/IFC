The _IfcWallElementedCase_ defines a wall with certain constraints for the provision of its components. The _IfcWallElementedCase_ handles all cases of walls, that are decomposed into parts:

* having components being assigned to the _IfcWallElementedCase_ using the _IfcRelAggregates_ relationship accessible by the inverse relationship _IsDecomposedBy_.
* applying the constraint that the parts within the decomposition shall be of type _IfcMember_, _IfcPlate_, _IfcBuildingElementPart_ or _IfcBuildingElementProxy_.

> HISTORY&nbsp; New entity in IFC4.

{ .use-head}
Property Set Use Definition:

The property sets relating to the _IfcWallElementedCase_ are defined at the supertype _IfcWall_.

> NOTE&nbsp; The parts within the decomposition relationship may define their own property sets.

{ .use-head}
Quantity Use Definition:

The quantities relating to the _IfcWallElementedCase_ are defined at the supertype _IfcWall_.

> NOTE&nbsp; The parts within the decomposition relationship may define their own individual quantities.

{ .use-head}
Voiding Use Definition:

As shown in Figure 1, openings within the composite wall are directly assigned to _IfcWallElementedCase_ using _IfcRelVoidsElement_ pointing to _IfcOpeningElement_ and apply to all aggregated parts. If individual parts have cutting and other voiding features, then the decomposed parts have a separate voiding relationship _IfcRelVoidsElement_ pointing to _IfcVoidingFeature_.

!["voiding"](../../../../../../figures/ifcwallelementedcase_fig01.png "Figure 1 &mdash; Wall elemented voiding")

**_Geometric Representation_**

The standard geometric representation of _IfcWallElementedCase_ is defined using the following multiple shape representations for its definition:

* **Axis**: A two-dimensional open curve being a subtype of _IfcBoundedCurve_ defining the axis for the elemented wall. It maybe used as a simplified representation directly at the elemented wall.
* **Surface**: A three-dimensional surface being a subtype of _IfcBoundedSurface_ defining the reference surface for the elemented wall. It maybe used as a simplified representation directly at the elemented wall.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcBuildingElement_: [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)
* _IfcWall_: [Object Typing](../../templates/object-typing.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Quantity Sets](../../templates/quantity-sets.htm), [Material Layer Set](../../templates/material-layer-set.htm), [Path Connectivity](../../templates/path-connectivity.htm), [Spatial Containment](../../templates/spatial-containment.htm), [Axis 2D Geometry](../../templates/axis-2d-geometry.htm), [Body SweptSolid Geometry](../../templates/body-sweptsolid-geometry.htm), [Body Clipping Geometry](../../templates/body-clipping-geometry.htm), [Element Voiding](../../templates/element-voiding.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcwallelementedcase.htm)

{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcmember.htm">IfcMember</a></td><td>Studs, sole plates, top plates.</td></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcplate.htm">IfcPlate</a></td><td>Sheathing, panels, drywall.</td></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedcomponentelements/lexical/ifcbuildingelementpart.htm">IfcBuildingElementPart</a></td><td>Insulation, other elements.</td></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcbeam.htm">IfcBeam</a></td><td>Lintels over doors or windows.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcWallElementedCase Object Aggregation</p></td></tr></table>

  
  
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
<tr><td><p class="table">Table 2 &mdash; IfcWallElementedCase Product Placement</p></td></tr></table>

The use of local placement is defined at the supertype _IfcWall_. The local placement of the _IfcWallElementedCase_ defines the parent coordinate systems for the parts within the decomposition. All parts shall be positioned relative to the _IfcWallElementedCase_.

  
  
{ .use-head}
Surface Geometry

The [Surface Geometry](../../templates/surface-geometry.htm) concept applies to this entity.

> NOTE&nbsp; The 'Surface' can be used to define a surfacic model of the building (e.g. for analytical purposes, or for reduced Level of Detail representation). It could suppress the geometric details of the parts in the decomposition.

> NOTE&nbsp; It is invalid to exchange a 'Body' shape representation of an _IfcWallElementedCase_. The body geometry is defined by the parts within the decomposition.
