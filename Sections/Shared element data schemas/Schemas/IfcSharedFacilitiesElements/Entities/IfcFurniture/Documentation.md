Furniture defines complete furnishings such as a table, desk, chair, or cabinet, which may or may not be permanently attached to a building structure.

Occurrences of furniture that are built in (where the property _Pset_FurnitureTypeCommon.IsBuiltIn_ is asserted to be TRUE) should have their connection relationship with a building element occurrence defined through the _IfcRelConnectsElements_ relationship.

> HISTORY&nbsp; New entity in IFC2x2.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcFurnishingElement_: [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcfurniture.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcfurnituretype.htm">IfcFurnitureType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcFurniture Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcfurnituretypeenum.htm">CHAIR</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_FurnitureTypeChair.xml">Pset_FurnitureTypeChair</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_FurnitureTypeCommon.xml">Pset_FurnitureTypeCommon</a></td></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcfurnituretypeenum.htm">DESK</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_FurnitureTypeDesk.xml">Pset_FurnitureTypeDesk</a></td></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcfurnituretypeenum.htm">FILECABINET</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_FurnitureTypeFileCabinet.xml">Pset_FurnitureTypeFileCabinet</a></td></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcfurnituretypeenum.htm">TABLE</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_FurnitureTypeTable.xml">Pset_FurnitureTypeTable</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcFurniture Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Finish</td><td>The finish, typically at visible aspects of the furniture.</td></tr>
<tr><td>Frame</td><td>The frame from which the object is constructed.</td></tr>
<tr><td>Hardware</td><td>Finiish hardware such as knobs or handles.</td></tr>
<tr><td>Padding</td><td>Padding such as cushions.</td></tr>
<tr><td>Panel</td><td>Panels such as glass.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcFurniture Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedfacilitieselements/lexical/ifcsystemfurnitureelement.htm">IfcSystemFurnitureElement</a></td><td>Modular furniture may be aggregated into components.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcFurniture Object Aggregation</p></td></tr></table>