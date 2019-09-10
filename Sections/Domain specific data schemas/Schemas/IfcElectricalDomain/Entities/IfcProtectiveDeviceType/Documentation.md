An _IfcProtectiveDeviceType_ is a device that breaks an electrical circuit when a stated electric current that passes through it is exceeded.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2 </font>
> 


****Use Definitions****

An _IfcProtectiveDeviceType_ is a subtype of IfcFlowControllerType that provides for various devices that ensure the safety of an electrical circuit.

Usage of _IfcProtectiveDeviceType_ defines the parameters for one or more occurrences of _IfcFlowController_. Parameters are specified through property sets that are enumerated in the _IfcIfcProtectiveDeviceTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcProtectiveDeviceType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcProtectiveDeviceType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_ProtectiveDeviceTypeCommon](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeCommon.xml): property set for properties that are common to all types of protective device, if available 
* [Pset_ProtectiveDeviceTypeCircuitBreaker](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeCircuitBreaker.xml): specific property set for the properties of a circuit breaker , if available 
* [Pset_ProtectiveDeviceTypeEarthFailureDevice](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeEarthFailureDevice.xml): specific property set for the properties of an earth failure device, if available 
* [Pset_ProtectiveDeviceTypeFuseDisconnector](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeFuseDisconnector.xml): specific property set for the properties of a fuse disconnector, if available 
* [Pset_ProtectiveDeviceTypeResidualCurrentCircuitBreaker](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeResidualCurrentCircuitBreaker.xml): specific property set for the properties of a residual current circuit breaker, if available 
* [Pset_ProtectiveDeviceTypeResidualCurrentSwitch](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeResidualCurrentSwitch.xml): specific property set for the properties of a residual current switch, if available 
* [Pset_ProtectiveDeviceTypeVaristor](../../psd/IfcElectricalDomain/Pset_ProtectiveDeviceTypeVaristor.xml): specific property set for the properties of a varistor, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.