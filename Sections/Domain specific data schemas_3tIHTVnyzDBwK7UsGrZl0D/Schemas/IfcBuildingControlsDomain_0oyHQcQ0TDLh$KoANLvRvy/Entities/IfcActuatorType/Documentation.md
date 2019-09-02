An _IfcActuatorType_ defines a particular type of actuating device that is typically used in a control system such as a building automation control system.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcActuatorType_ provides for all forms of actuator.

Usage of _IfcActuatorType_ defines the parameters for one or more occurrences of _IfcDistributionControlElement_. Parameters may be specified through property sets that are enumerated in the _IfcActuatorTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcActuatorType_ defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcActuatorType_ are part of this IFC release:

* [Pset_ActuatorTypeCommon](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypeCommon.xml): property set for the properties common to all types of actuator, if available 
* [Pset_ActuatorTypeLinearActuation](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypeLinearActuation.xml): specific property set for the properties of a linear actuator, if available 
* [Pset_ActuatorTypeRotationalActuation](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypeRotationalActuation.xml): specific property set for the properties of a rotational actuator, if available 
* [Pset_ActuatorTypeElectricActuator](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypeElectricActuator.xml): specific property set for the properties of an electrical actuator, if available 
* [Pset_ActuatorTypeHydraulicActuator](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypeHydraulicActuator.xml): specific property set for the properties of an hydraulic actuator, if available 
* [Pset_ActuatorTypePneumaticActuator](../../psd/IfcBuildingControlsDomain/Pset_ActuatorTypePneumaticActuator.xml): specific property set for the properties of a pneumatic actuator, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.