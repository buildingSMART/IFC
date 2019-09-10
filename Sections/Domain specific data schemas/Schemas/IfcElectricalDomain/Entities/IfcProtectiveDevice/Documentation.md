A protective device breaks an electrical circuit when a stated electric current that passes through it is exceeded.

A protective device provides protection against electrical current only (not as a general protective device). It may be used to represent the complete set of elements including both the tripping unit and the breaking unit that provide the protection. This may be particularly useful at earlier stages of design where the approach to breaking the electrical supply may be determined but the method of tripping may not. Alternatively, this entity may be used to specifically represent the breaking unit alone (in which case the tripping unit will also be specifically identified). This entity is specific to dedicated protective devices and excludes electrical outlets that may have circuit protection.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcprotectivedevice.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetype.htm">IfcProtectiveDeviceType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcProtectiveDevice Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceBreakerUnitI2TCurve.xml">Pset_ProtectiveDeviceBreakerUnitI2TCurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceBreakerUnitI2TFuseCurve.xml">Pset_ProtectiveDeviceBreakerUnitI2TFuseCurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceBreakerUnitIPICurve.xml">Pset_ProtectiveDeviceBreakerUnitIPICurve</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">CIRCUITBREAKER</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceBreakerUnitTypeMCB.xml">Pset_ProtectiveDeviceBreakerUnitTypeMCB</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceBreakerUnitTypeMotorProtection.xml">Pset_ProtectiveDeviceBreakerUnitTypeMotorProtection</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingCurve.xml">Pset_ProtectiveDeviceTrippingCurve</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">CIRCUITBREAKER</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeCircuitBreaker.xml">Pset_ProtectiveDeviceTypeCircuitBreaker</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeCommon.xml">Pset_ProtectiveDeviceTypeCommon</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">EARTHLEAKAGECIRCUITBREAKER</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeEarthLeakageCircuitBreaker.xml">Pset_ProtectiveDeviceTypeEarthLeakageCircuitBreaker</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">FUSEDISCONNECTOR</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeFuseDisconnector.xml">Pset_ProtectiveDeviceTypeFuseDisconnector</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">RESIDUALCURRENTCIRCUITBREAKER</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeResidualCurrentCircuitBreaker.xml">Pset_ProtectiveDeviceTypeResidualCurrentCircuitBreaker</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">RESIDUALCURRENTSWITCH</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeResidualCurrentSwitch.xml">Pset_ProtectiveDeviceTypeResidualCurrentSwitch</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetypeenum.htm">VARISTOR</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTypeVaristor.xml">Pset_ProtectiveDeviceTypeVaristor</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcProtectiveDevice Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcelectricaldomain/Qto_ProtectiveDeviceBaseQuantities.xml">Qto_ProtectiveDeviceBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcProtectiveDevice Quantity Sets</p></td></tr></table>

  
  
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
<tr><td><p class="table">Table 4 &mdash; IfcProtectiveDevice Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>Line</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The supply line, typically connected from a slot in a distribution board.</td></tr>
<tr><td>&nbsp;</td><td>Load</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The load protected by this device, typically a cable connected to a device or the first junction box of a circuit.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcProtectiveDevice Port Nesting</p></td></tr></table>
