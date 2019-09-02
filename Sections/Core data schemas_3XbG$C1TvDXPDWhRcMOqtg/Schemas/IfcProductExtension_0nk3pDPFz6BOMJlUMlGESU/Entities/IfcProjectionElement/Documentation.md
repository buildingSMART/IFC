The projection element is a specialization of the general feature element to represent projections applied to building elements. It represents a solid attached to any element that has physical manifestation.

> EXAMPLE&nbsp; A wall projection such as a pilaster strip is handled by _IfcProjectionElement_

> NOTE&nbsp; View definitions or implementer agreements may restrict the types of elements to which _IfcProjectionElement_ can be applied.

An _IfcProjectionElement_ has to be linked to a element (all subtypes of _IfcElement_) by using the _IfcRelProjectsElement_ relationship. Its existence depends on the existence of the master element. The relationship implies a Boolean union operation between the volume of the projection element and the volume of the element.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _PredefinedType_ has been added at the end of attribute list.

{ .use-head}
Containment Use Definition

The _IfcProjectionElement_ shall not participate in the containment relationship, i.e. it is not linked directly to the spatial structure of the project. It has a mandatory _ProjectsElements_ inverse relationship pointing to the _IfcElement_ that is contained in the spatial structure.

* The inverse relationship _ContainedInStructure_ shall be NIL.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcFeatureElement_: [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcprojectionelement.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Condition.xml">Pset_Condition</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactIndicators.xml">Pset_EnvironmentalImpactIndicators</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactValues.xml">Pset_EnvironmentalImpactValues</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerOccurrence.xml">Pset_ManufacturerOccurrence</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerTypeInformation.xml">Pset_ManufacturerTypeInformation</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedmgmtelements/Pset_PackingInstructions.xml">Pset_PackingInstructions</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLife.xml">Pset_ServiceLife</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Warranty.xml">Pset_Warranty</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcProjectionElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcproductextension/Qto_ProjectionElementBaseQuantities.xml">Qto_ProjectionElementBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcProjectionElement Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Relative</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>Relative placement according to position and rotation relative to container.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>&nbsp;</td><td>Absolute placement according to position and rotation of world coordinate system.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifcgridplacement.htm">IfcGridPlacement</a></td><td>&nbsp;</td><td>Placement according to grid intersection.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcProjectionElement Product Placement</p></td></tr></table>

The local placement for _IfcOpeningRecess_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ should point to the local placement of the same element, to which the projection adds, i.e. referred to by _ProjectsElement.RelatingBuildingElement_.

  
  
{ .use-head}
Body Geometry

The [Body Geometry](../../templates/body-geometry.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcProjectionElement Body Geometry</p></td></tr></table>

The geometric representation of _IfcProjectionElement_ is defined using the swept area solid geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required.
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded horizontally (that is, perpendicular to the extrusion direction of the modified element), such as for wall projections, or vertically (that is, in the extrusion direction of the projected element), such as for floor projections.

As shown in Figure 1, the following interpretation of dimension parameter applies for rectangular projection:

* _IfcRectangleProfileDef.YDim_ interpreted as projection width
* _IfcRectangleProfileDef.XDim_ interpreted as projection height
* _IfcExtrudedAreaSolid.Depth_ is interpreted as projection depth

> NOTE&nbsp; Rectangles are now defined centric, the placement location has to be set: > * _IfcCartesianPoint_(XDim/2,YDim/2)

> NOTE&nbsp; The local placement directions for the _IfcProjectionElement_ are only given as an example, other directions are valid as well.

!["projection"](../../../figures/IfcProjectionElement-Layout1.png "Figure 1 &mdash; Projection representation")

The general b-rep geometric representation of _IfcProjectionElement_ is defined using the Brep geometry. The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'Brep'