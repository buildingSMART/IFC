**Definition from BS6100 310 5201**: An _IfcElectricMotorType_ defines a particular type of engine that is a machine for converting electrical energy into mechanical energy.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcElectricMotorType_ is a subtype of _IfcEnergyConversionDeviceType_ that provides for all forms of electric motor.

Usage of _IfcElectricMotorType_ defines the parameters for one or more occurrences of _IfcEnergyConversionDevice_.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricMotorType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricMotorType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_ElectricMotorTypeCommon](../../psd/IfcElectricalDomain/Pset_ElectricMotorTypeCommon.xml): property set for properties that are common to all types of electrical motor, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.