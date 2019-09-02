An _IfcElectricFlowStorageDeviceType_ is a device in which electrical energy is stored and from which energy may be progressively released.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2. </font>
> 


****Use Definitions****

An _IfcElectricFlowStorageDeviceType_ is a subtype of IfcFlowStorageDeviceType that provides for various devices that store electrical energy.

Usage of _IfcElectricFlowStorageDeviceType_ defines the parameters for one or more occurrences of _IfcFlowStorageDevice_.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricFlowStorageDeviceType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricFlowStorageDeviceType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.