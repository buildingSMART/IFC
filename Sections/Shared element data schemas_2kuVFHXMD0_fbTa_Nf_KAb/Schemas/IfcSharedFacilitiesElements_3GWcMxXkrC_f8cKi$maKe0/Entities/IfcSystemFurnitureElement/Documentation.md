A system furniture element defines components of modular furniture which are not directly placed in a building structure but aggregated inside furniture.

> HISTORY&nbsp; New entity in IFC2x2.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcFurnishingElement_: [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcsystemfurnitureelement.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcsystemfurnitureelementtype.htm">IfcSystemFurnitureElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcSystemFurnitureElement Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_SystemFurnitureElementTypeCommon.xml">Pset_SystemFurnitureElementTypeCommon</a></td></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcsystemfurnitureelementtypeenum.htm">PANEL</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_SystemFurnitureElementTypePanel.xml">Pset_SystemFurnitureElementTypePanel</a></td></tr>
<tr><td><a href="../../ifcsharedfacilitieselements/lexical/ifcsystemfurnitureelementtypeenum.htm">WORKSURFACE</a></td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_SystemFurnitureElementTypeWorkSurface.xml">Pset_SystemFurnitureElementTypeWorkSurface</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcSystemFurnitureElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Finish</td><td>The finish, typically at visible aspects of the furniture.</td></tr>
<tr><td>Frame</td><td>The frame from which the object is constructed.</td></tr>
<tr><td>Hardware</td><td>Finish hardware such as knobs or handles.</td></tr>
<tr><td>Padding</td><td>Padding such as cushions.</td></tr>
<tr><td>Panel</td><td>Panels such as glass.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcSystemFurnitureElement Material Constituents</p></td></tr></table>