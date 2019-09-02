An _IfcLightFixtureType_ is a container type that is designed for the purpose of housing one or more lamps and the devices that control, restrict or vary their emission.

> <font color="#0000ff" size="-1">HISTORY:
New class in IFC 2x2.</font>

****Use Definitions****

An _IfcLightFixtureType_ provides for all forms of light fixture and its usage defines the parameters for one or more occurrences of _IfcFlowTerminal_.

Instances of _IfcFlowTerminal_ that are defined as types of _IfcLightFixtureType_ have one or more instances of _IfcFlowTerminal_ that are defined as types of _IfcLampType_ connected using instances of _IfcDistributionPort_.

Rendering using lighting data is achieved using light source entities within the presentation capabilities of IFC.

****Property Set Use Definition****:

The property sets relating to the _IfcLightFixtureType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcLightFixtureType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_LightFixtureTypeCommon](../../psd/IfcElectricalDomain/Pset_LightFixtureTypeCommon.xml): property set for properties that are common to all types of light fixture, if available 
* [Pset_LightFixtureTypeThermal](../../psd/IfcElectricalDomain/Pset_LightFixtureTypeThermal.xml): specific property set for the thermal properties of a light fixture, if available 
* [Pset_LightFixtureTypeExitSign](../../psd/IfcElectricalDomain/Pset_LightFixtureTypeExitSign.xml): specific property set for the properties of an exit sign, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.