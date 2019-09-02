A reinforcing mesh is a series of longitudinal and transverse wires or bars of various gauges, arranged at right angles to each other and welded at all points of intersection; usually used for concrete slab reinforcement. It is also known as welded wire fabric. In scope are plane meshes as well as bent meshes.

> HISTORY&nbsp; New entity in IFC2x2

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; All attributes are optional now. Several attributes are deprecated; their information is now provided by _IfcReinforcingMeshType_. Attribute _PredefinedType_ added.

{ .use-head}
Geometry Use Definition

Placement and representation are defined at the supertype _IfcElementComponent_.

The representation map of a mapped 'Outline' representation should contain a representation of type 'Curve3D' which holds an _IfcPolyline_.

The representation map of a mapped 'Body' representation should contain a representation of type 'AdvancedSweptSolid' which holds multiple _IfcSweptDiskSolid_ (including subtype _IfcSweptDiskSolidPolygonal_).

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm)
* _IfcElementComponent_: [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcreinforcingmesh.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcstructuralelementsdomain/lexical/ifcreinforcingmeshtype.htm">IfcReinforcingMeshType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcReinforcingMesh Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

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
<tr><td><p class="table">Table 2 &mdash; IfcReinforcingMesh Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td>Qto_ReinforcingElementBaseQuantities</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcReinforcingMesh Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Body Geometry

The [Body Geometry](../../templates/body-geometry.htm) concept applies to this entity.

The representation map referenced by a 'Body' 'MappedRepresentation' could contain a representation of type 'AdvancedSweptSolid' which holds an _IfcSweptDiskSolid_ (including subtype _IfcSweptDiskSolidPolygonal_). Multiple _IfcMappedItem_'s can be used to represent the bars within a mesh as one occurrence of _IfcReinforcingMesh_.