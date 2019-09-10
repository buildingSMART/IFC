An _IfcSensorType_ defines a particular type of sensor which is used for detection in a control system such as a building automation control system.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcSensorType_ provides for all forms of sensor.

Usage of _IfcSensorType_ defines the parameters for one or more occurrences of _IfcDistributionControlElement_. Parameters are specified through property sets that are enumerated in the _IfcSensorTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcSensorType_ defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcSensorType_ are part of this IFC release:

* [Pset_SensorTypeCO2Sensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeCO2Sensor.xml): specific property set for the properties of a CO2 sensor, if available 
* [Pset_SensorTypeFireSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeFireSensor.xml): specific property set for the properties of a fire sensor, if available 
* [Pset_SensorTypeGasSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeGasSensor.xml): specific property set for the properties of a gas sensor, if available
* [Pset_SensorTypeHeatSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeHeatSensor.xml): specific property set for the properties of a heat sensor, if available
* [Pset_SensorTypeHumiditySensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeHumiditySensor.xml): specific property set for the properties of a humidity sensor, if available 
* [Pset_SensorTypeLightSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeLightSensor.xml): specific property set for the properties of a light sensor, if available
* [Pset_SensorTypeMovementSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeMovementSensor.xml): specific property set for the properties of a movement sensor, if available
* [Pset_SensorTypePressureSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypePressureSensor.xml): specific property set for the properties of a pressure sensor, if available 
* [Pset_SensorTypeSmokeSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeSmokeSensor.xml): specific property set for the properties of a smoke sensor, if available
* [Pset_SensorTypeSoundSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeSoundSensor.xml): specific property set for the properties of a sound sensor, if available
* [Pset_SensorTypeTemperatureSensor](../../psd/IfcBuildingControlsDomain/Pset_SensorTypeTemperatureSensor.xml): specific property set for the properties of a temperature sensor, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.
