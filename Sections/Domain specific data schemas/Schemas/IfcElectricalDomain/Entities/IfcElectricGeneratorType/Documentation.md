An _IfcElectricGeneratorType_ defines a particular type of engine that is a machine for converting mechanical energy into electrical energy.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions,****

An _IfcElectricGeneratorType_ is a subtype of IfcEnergyConversionDeviceType that provides for all forms of electric engine.

Usage of _IfcElectricGeneratorType_ defines the parameters for one or more occurrences of _IfcEnergyConversionDevice_. No predefined types of electrical generator are specified at this stage. Use the _IfcElectricalGeneratorType.Name_ and _IfcElectricalGeneratorType.Description_ attributes to further qualify a generator.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricGeneratorType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricGeneratorType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_ElectricGeneratorTypeCommon](../../psd/IfcElectricalDomain/Pset_ElectricGeneratorTypeCommon.xml): property set for properties that are common to all types of electrical generator, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.