An _IfcLampType_ is a type of device that is designed to emit light.

> <font color="#0000ff" size="-1">HISTORY:
New entity in IFC 2x2 Addendum 1.</font>

****Use Definitions****

An _IfcLampType_ provides for all forms of lamp and its usage defines the parameters for one or more occurrences of _IfcFlowTerminal_.

Instances of _IfcFlowTerminal_ that are defined as types of _IfcLampType_ are connected via instances of _IfcDistributionPort_ to an instance of _IfcFlowTerminal_ that is defined as a type of _IfcLightFixtureType_.

Rendering using lighting data is achieved using light source entities within the presentation capabilities of IFC.

****Property Set Use Definition****:

The property sets relating to the _IfcLampType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcLampType_ are part of this IFC release:

* [Pset_LampTypeCommon](../../psd/IfcElectricalDomain/Pset_LampTypeCommon.xml): property set for properties that are common to all types of lamp installed within a light fixture, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.