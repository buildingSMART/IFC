﻿An actuator is a mechanical device for moving or controlling a mechanism or system. An actuator takes energy, usually created by air, electricity, or liquid, and converts that into some kind of motion.

> HISTORY&nbsp; New entity in IFC4

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionControlElement_: [Object Classification](../../templates/object-classification.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcactuator.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcactuatortype.htm">IfcActuatorType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributioncontrolelementtype.htm">IfcDistributionControlElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcActuator Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorPHistory.xml">Pset_ActuatorPHistory</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypeCommon.xml">Pset_ActuatorTypeCommon</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcactuatortypeenum.htm">ELECTRICACTUATOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypeElectricActuator.xml">Pset_ActuatorTypeElectricActuator</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcactuatortypeenum.htm">HYDRAULICACTUATOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypeHydraulicActuator.xml">Pset_ActuatorTypeHydraulicActuator</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypeLinearActuation.xml">Pset_ActuatorTypeLinearActuation</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcactuatortypeenum.htm">PNEUMATICACTUATOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypePneumaticActuator.xml">Pset_ActuatorTypePneumaticActuator</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_ActuatorTypeRotationalActuation.xml">Pset_ActuatorTypeRotationalActuation</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcActuator Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcbuildingcontrolsdomain/Qto_ActuatorBaseQuantities.xml">Qto_ActuatorBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcActuator Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcActuator Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">Sink</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">Signal</a></td><td>Receives signal.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcActuator Port Nesting</p></td></tr></table>

  
  
{ .use-head}
Control Flow

The [Control Flow](../../templates/control-flow.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowcontroller.htm">IfcFlowController</a></td><td>Indicates a connected valve, damper, or switch controlled by the actuator.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcActuator Control Flow</p></td></tr></table>