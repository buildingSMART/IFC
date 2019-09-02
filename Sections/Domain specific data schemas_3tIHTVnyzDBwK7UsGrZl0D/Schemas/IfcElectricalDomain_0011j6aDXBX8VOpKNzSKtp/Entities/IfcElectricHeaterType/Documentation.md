An _IfcElectricHeaterType_ is a device that emits electrical energy as heat.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2 </font>
> 


****Use Definitions****

An _IfcElectricHeaterType_ is a subtype of IfcEnergyConversionDeviceType that provides for various devices that emit electrical energy as heat.

Usage of _IfcElectricHeaterType_ defines the parameters for one or more occurrences of _IfcEnergyConversionDevice_. Parameters are specified through property sets that are enumerated in the _IfcElectricHeaterTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricHeaterType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricHeaterType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_ElectricHeaterTypeElectricalCableHeater](../../psd/IfcElectricalDomain/Pset_ElectricHeaterTypeElectricalCableHeater.xml): specific property set for the properties of an electrical cable heater emitting heat along its length, if available 
* [Pset_ElectricHeaterTypeElectricalMatHeater](../../psd/IfcElectricalDomain/Pset_ElectricHeaterTypeElectricalMatHeater.xml): specific property set for the properties of an electrical mat heater emitting heat over its complete coverage area, if available 
* [Pset_ElectricHeaterTypeElectricalPointHeater](../../psd/IfcElectricalDomain/Pset_ElectricHeaterTypeElectricalPointHeater.xml): specific property set for the properties of an electrical point heater emitting heat at the point of its location, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.