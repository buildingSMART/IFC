A protective device tripping unit breaks an electrical circuit at a separate breaking unit when a stated electric current that passes through the unit is exceeded.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcprotectivedevicetrippingunit.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetrippingunittype.htm">IfcProtectiveDeviceTrippingUnitType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributioncontrolelementtype.htm">IfcDistributionControlElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcProtectiveDeviceTrippingUnit Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingFunctionGCurve.xml">Pset_ProtectiveDeviceTrippingFunctionGCurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingFunctionICurve.xml">Pset_ProtectiveDeviceTrippingFunctionICurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingFunctionLCurve.xml">Pset_ProtectiveDeviceTrippingFunctionLCurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingFunctionSCurve.xml">Pset_ProtectiveDeviceTrippingFunctionSCurve</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitCurrentAdjustment.xml">Pset_ProtectiveDeviceTrippingUnitCurrentAdjustment</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTimeAdjustment.xml">Pset_ProtectiveDeviceTrippingUnitTimeAdjustment</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTypeCommon.xml">Pset_ProtectiveDeviceTrippingUnitTypeCommon</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetrippingunittypeenum.htm">ELECTROMAGNETIC</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTypeElectroMagnetic.xml">Pset_ProtectiveDeviceTrippingUnitTypeElectroMagnetic</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetrippingunittypeenum.htm">ELECTRONIC</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTypeElectronic.xml">Pset_ProtectiveDeviceTrippingUnitTypeElectronic</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetrippingunittypeenum.htm">RESIDUALCURRENT</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTypeResidualCurrent.xml">Pset_ProtectiveDeviceTrippingUnitTypeResidualCurrent</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevicetrippingunittypeenum.htm">THERMAL</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_ProtectiveDeviceTrippingUnitTypeThermal.xml">Pset_ProtectiveDeviceTrippingUnitTypeThermal</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcProtectiveDeviceTrippingUnit Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcelectricaldomain/Qto_ProtectiveDeviceTrippingUnitBaseQuantities.xml">Qto_ProtectiveDeviceTrippingUnitBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcProtectiveDeviceTrippingUnit Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Control Flow

The [Control Flow](../../templates/control-flow.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcprotectivedevice.htm">IfcProtectiveDevice</a></td><td>The corresponding breaker unit for breaking the circuit.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcProtectiveDeviceTrippingUnit Control Flow</p></td></tr></table>