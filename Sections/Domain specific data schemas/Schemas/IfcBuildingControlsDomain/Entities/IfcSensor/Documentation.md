A sensor is a device that measures a physical quantity and converts it into a signal which can be read by an observer or by an instrument.

> HISTORY&nbsp; New entity in IFC4

{ .note}
> 

{ .use-head}
Connection Use Definition

The **IfcSensor** may be connected to other objects as follows using the indicated relationship:

* **[IfcDistributionFlowElement](../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelement.htm)** ([IfcRelFlowControlElements](../../ifcsharedbldgserviceelements/lexical/ifcrelflowcontrolelements.htm)): Sensors may be connected to a flow element for which an aspect of the fluid or flow is measured.
* **[IfcElement](../../ifcproductextension/lexical/ifcelement.htm)** ([IfcRelConnectsElements](../../ifcproductextension/lexical/ifcrelconnectselements.htm)): Sensors may be attached to the exterior of an element.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionControlElement_: [Object Classification](../../templates/object-classification.htm), [Product Assignment](../../templates/product-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcsensor.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortype.htm">IfcSensorType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributioncontrolelementtype.htm">IfcDistributionControlElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcSensor Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorPHistory.xml">Pset_SensorPHistory</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeCommon.xml">Pset_SensorTypeCommon</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">CONDUCTANCESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeConductanceSensor.xml">Pset_SensorTypeConductanceSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">CONTACTSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeContactSensor.xml">Pset_SensorTypeContactSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">FIRESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeFireSensor.xml">Pset_SensorTypeFireSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">FLOWSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeFlowSensor.xml">Pset_SensorTypeFlowSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">GASSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeGasSensor.xml">Pset_SensorTypeGasSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">HEATSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeHeatSensor.xml">Pset_SensorTypeHeatSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">HUMIDITYSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeHumiditySensor.xml">Pset_SensorTypeHumiditySensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">IONCONCENTRATIONSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeIonConcentrationSensor.xml">Pset_SensorTypeIonConcentrationSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">LEVELSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeLevelSensor.xml">Pset_SensorTypeLevelSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">LIGHTSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeLightSensor.xml">Pset_SensorTypeLightSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">MOISTURESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeMoistureSensor.xml">Pset_SensorTypeMoistureSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">MOVEMENTSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeMovementSensor.xml">Pset_SensorTypeMovementSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">PHSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypePHSensor.xml">Pset_SensorTypePHSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">PRESSURESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypePressureSensor.xml">Pset_SensorTypePressureSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">RADIATIONSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeRadiationSensor.xml">Pset_SensorTypeRadiationSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">RADIOACTIVITYSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeRadioactivitySensor.xml">Pset_SensorTypeRadioactivitySensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">SMOKESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeSmokeSensor.xml">Pset_SensorTypeSmokeSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">SOUNDSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeSoundSensor.xml">Pset_SensorTypeSoundSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">TEMPERATURESENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeTemperatureSensor.xml">Pset_SensorTypeTemperatureSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">WINDSENSOR</a></td><td><a href="../../psd/ifcbuildingcontrolsdomain/Pset_SensorTypeWindSensor.xml">Pset_SensorTypeWindSensor</a></td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">CO2SENSOR</a></td><td>Pset_SensorTypeCO2Sensor</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">FROSTSENSOR</a></td><td>Pset_SensorTypeFrostSensor</td></tr>
<tr><td><a href="../../ifcbuildingcontrolsdomain/lexical/ifcsensortypeenum.htm">IDENTIFIERSENSOR</a></td><td>Pset_SensorTypeIdentifierSensor</td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcSensor Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcbuildingcontrolsdomain/Qto_SensorBaseQuantities.xml">Qto_SensorBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcSensor Quantity Sets</p></td></tr></table>

  
  
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
<tr><td><p class="table">Table 4 &mdash; IfcSensor Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">SIGNAL</a></td><td>Transmits signal.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcSensor Port Nesting</p></td></tr></table>

  
  
{ .use-head}
Control Flow

The [Control Flow](../../templates/control-flow.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelement.htm">IfcDistributionFlowElement</a></td><td>Sensors may be connected to a flow element for which an aspect of the fluid or flow is measured.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcSensor Control Flow</p></td></tr></table>
