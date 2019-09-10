An _IfcElectricTimeControlType_ is a device that applies control to the provision or flow of electrical energy over time.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcElectricTimeControlType_ is a subtype of _IfcFlowControllerType_.

Usage of _IfcElectricTimeControlType_ defines the parameters for one or more occurrences of _IfcFlowController_.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricTimeControlType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricTimeControlType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.