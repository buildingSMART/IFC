A switch is used in a cable distribution system (electrical circuit) to control or modulate the flow of electricity.

Switches include those used for electrical power, communications, audio-visual, or other distribution system types as determined by the available ports.

> HISTORY&nbsp; New entity in IFC4

{ .note}
> 

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionFlowElement_: [Axis Geometry](../../templates/axis-geometry.htm), [Clearance Geometry](../../templates/clearance-geometry.htm), [Lighting Geometry](../../templates/lighting-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcswitchingdevice.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetype.htm">IfcSwitchingDeviceType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcSwitchingDevice Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeCommon.xml">Pset_SwitchingDeviceTypeCommon</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">CONTACTOR</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeContactor.xml">Pset_SwitchingDeviceTypeContactor</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">DIMMERSWITCH</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeDimmerSwitch.xml">Pset_SwitchingDeviceTypeDimmerSwitch</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">EMERGENCYSTOP</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeEmergencyStop.xml">Pset_SwitchingDeviceTypeEmergencyStop</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">KEYPAD</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeKeypad.xml">Pset_SwitchingDeviceTypeKeypad</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">MOMENTARYSWITCH</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeMomentarySwitch.xml">Pset_SwitchingDeviceTypeMomentarySwitch</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypePHistory.xml">Pset_SwitchingDeviceTypePHistory</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">SELECTORSWITCH</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeSelectorSwitch.xml">Pset_SwitchingDeviceTypeSelectorSwitch</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">STARTER</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeStarter.xml">Pset_SwitchingDeviceTypeStarter</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">SWITCHDISCONNECTOR</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeSwitchDisconnector.xml">Pset_SwitchingDeviceTypeSwitchDisconnector</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcswitchingdevicetypeenum.htm">TOGGLESWITCH</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_SwitchingDeviceTypeToggleSwitch.xml">Pset_SwitchingDeviceTypeToggleSwitch</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_SoundGeneration.xml">Pset_SoundGeneration</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcSwitchingDevice Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcelectricaldomain/Qto_SwitchingDeviceBaseQuantities.xml">Qto_SwitchingDeviceBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcSwitchingDevice Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
<tr><td>Conductor</td><td>Material from which the conductors are constructed.</td></tr>
<tr><td>Surface</td><td>Material from which the switch surface is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcSwitchingDevice Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>Line</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The supply line.</td></tr>
<tr><td>&nbsp;</td><td>Load</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The load controlled by the switch.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcSwitchingDevice Port Nesting</p></td></tr></table>