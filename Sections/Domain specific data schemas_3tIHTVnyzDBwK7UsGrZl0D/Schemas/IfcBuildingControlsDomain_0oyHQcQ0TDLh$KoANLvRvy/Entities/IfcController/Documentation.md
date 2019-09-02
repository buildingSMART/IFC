A controller is a device that monitors inputs and controls outputs within a building automation system.

A controller may be physical (having placement within a spatial structure) or logical (a software interface or aggregated within a programmable physical controller).

> HISTORY&nbsp; New entity in IFC4

{ .note}
> 

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionControlElement_: [Object Classification](../../templates/object-classification.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifccontroller.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertype.htm">IfcControllerType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributioncontrolelementtype.htm">IfcDistributionControlElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcController Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerPHistory.xml">Pset_ControllerPHistory</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeCommon.xml">Pset_ControllerTypeCommon</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">FLOATING</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeFloating.xml">Pset_ControllerTypeFloating</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">MULTIPOSITION</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeMultiPosition.xml">Pset_ControllerTypeMultiPosition</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeProgrammable.xml">Pset_ControllerTypeProgrammable</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROPORTIONAL</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeProportional.xml">Pset_ControllerTypeProportional</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">TWOPOSITION</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ControllerTypeTwoPosition.xml">Pset_ControllerTypeTwoPosition</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ElectricalDeviceCommon.xml">Pset_ElectricalDeviceCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcController Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcbuildingcontrolsdomain/Qto_ControllerBaseQuantities.xml">Qto_ControllerBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcController Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontroller.htm">IfcController</a></td><td>May contain IfcController components. Programmable Logic Controllers may be decomposed into logical elements for values and operations.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcController Object Aggregation</p></td></tr></table>

Figure 1 illustrates controller composition use.

!["Composition Use Definition"](../../../figures/ifccontroller-Composition.png "Figure 1 &mdash; Controller composition use")

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcController Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">FLOATING</a></td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the first parameter.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">FLOATING</a></td><td>Modifier</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the second parameter (if applicable).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">FLOATING</a></td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Sets the output value.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">MULTIPOSITION</a></td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the first parameter.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">MULTIPOSITION</a></td><td>Modifier</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the second parameter (if applicable).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">MULTIPOSITION</a></td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Sets the output value.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td>Power</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>Receives electrical power.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td>Control</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">CONTROL</a></td><td>Direct communication to the device (e.g. serial port).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td>Data</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DATA</a></td><td>Network communication to the device (e.g. TCP/IP network).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td>Input#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Analog or digital inputs.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROGRAMMABLE</a></td><td>Output#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Analog or digital outputs.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROPORTIONAL</a></td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the first parameter.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROPORTIONAL</a></td><td>Modifier</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the second parameter (if applicable).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">PROPORTIONAL</a></td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Sets the output value.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">TWOPOSITION</a></td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the first parameter.</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">TWOPOSITION</a></td><td>Modifier</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Receives the second parameter (if applicable).</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifccontrollertypeenum.htm">TWOPOSITION</a></td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Sets the output value.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcController Port Nesting</p></td></tr></table>