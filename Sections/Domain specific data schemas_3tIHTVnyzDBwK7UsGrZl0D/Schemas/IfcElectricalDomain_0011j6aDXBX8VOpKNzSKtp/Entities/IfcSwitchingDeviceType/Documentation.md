An _IfcSwitchingDeviceType_ defines a particular type of switch which is a mechanically operated contactor.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2 </font>
> 


****Use Definitions****

An _IfcSwitchingDeviceType_ is a subtype of _IfcFlowControllerType_ that provides for all forms of switch.

Usage of _IfcSwitchingDeviceType_ defines the parameters for one or more occurrences of _IfcFlowController_. Parameters are specified through property sets that are enumerated in the _IfcSwitchingDeviceTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcSwitchingDeviceType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcSwitchingDeviceType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_SwitchingDeviceTypeCommon](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeCommon.xml): property set for properties that are common to all types of switching device, if available 
* [Pset_SwitchingDeviceTypeContactor](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeContactor.xml): specific property set for the properties of a contactor , if available 
* [Pset_SwitchingDeviceTypeEmergencyStop](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeEmergencyStop.xml): specific property set for the properties of an emergency stop device, if available 
* [Pset_SwitchingDeviceTypeStarter](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeStarter.xml): specific property set for the properties of a starter, if available 
* [Pset_SwitchingDeviceTypeSwitchDisconnector](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeSwitchDisconnector.xml): specific property set for the properties of a switch disconnector, if available 
* [Pset_SwitchingDeviceTypeToggleSwitch](../../psd/IfcElectricalDomain/Pset_SwitchingDeviceTypeToggleSwitch.xml): specific property set for the properties of a toggle switch, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.