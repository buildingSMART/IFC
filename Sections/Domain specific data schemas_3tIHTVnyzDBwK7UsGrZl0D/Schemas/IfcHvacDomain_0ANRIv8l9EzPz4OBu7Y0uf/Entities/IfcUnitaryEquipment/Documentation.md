Unitary equipment typically combine a number of components into a single product, such as air handlers, pre-packaged rooftop air-conditioning units, and split systems.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcunitaryequipment.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttype.htm">IfcUnitaryEquipmentType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcUnitaryEquipment Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRCONDITIONINGUNIT</a></td><td><a href="../../psd/ifchvacdomain/Pset_UnitaryEquipmentTypeAirConditioningUnit.xml">Pset_UnitaryEquipmentTypeAirConditioningUnit</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td><a href="../../psd/ifchvacdomain/Pset_UnitaryEquipmentTypeAirHandler.xml">Pset_UnitaryEquipmentTypeAirHandler</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_UnitaryEquipmentTypeCommon.xml">Pset_UnitaryEquipmentTypeCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcUnitaryEquipment Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifchvacdomain/Qto_UnitaryEquipmentBaseQuantities.xml">Qto_UnitaryEquipmentBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcUnitaryEquipment Quantity Sets</p></td></tr></table>

  
  
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
<tr><td><p class="table">Table 4 &mdash; IfcUnitaryEquipment Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcproductextension/lexical/ifcdistributionelement.htm">IfcDistributionElement</a></td><td>Unitary equipment (air handlers in particular) may elaborate contained elements such as dampers, fans, coils, sensors, actuators, and controllers. Such breakdown provides access to component information and tracking of performance history for embedded elements.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcUnitaryEquipment Object Aggregation</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>ReturnAirIn</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">AIRCONDITIONING</a></td><td>Return air entering mixture or exhausted.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>SupplyAirOut</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">AIRCONDITIONING</a></td><td>Chilled supply air.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>OutsideAirIn</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">VENTILATION</a></td><td>Outside air entering mixture.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>ExhaustAirOut</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">EXHAUST</a></td><td>Exhaust air leaving to outside.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>ChilledWaterIn</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">CHILLEDWATER</a></td><td>Chilled water entering cooling coil.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>ChilledWaterOut</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">CHILLEDWATER</a></td><td>Chilled water leaving cooling coil.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>HeatingIn</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">HEATING</a></td><td>Steam entering heating coil.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>HeatingOut</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">HEATING</a></td><td>Steam leaving heating coil.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>Power</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>Electrical power source.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcunitaryequipmenttypeenum.htm">AIRHANDLER</a></td><td>Control</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">CONTROL</a></td><td>Control system communication.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcUnitaryEquipment Port Nesting</p></td></tr></table>