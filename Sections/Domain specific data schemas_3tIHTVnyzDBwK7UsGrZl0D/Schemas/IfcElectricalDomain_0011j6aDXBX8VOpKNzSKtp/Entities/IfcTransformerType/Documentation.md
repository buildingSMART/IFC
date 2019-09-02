An _IfcTransformerType_ defines a particular type of transformer that is an inductive stationary device that transfers electrical energy from one circuit to another.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcTransformerType_ is a subtype of IfcEnergyConversionDeviceType that provides for all forms of transformer.

Usage of _IfcTransformerType_ defines the parameters for one or more occurrences of _IfcEnergyConversionDevice_. Parameters are specified through a common property set.

****Property Set Use Definition****:

The property sets relating to the _IfcTransformerType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcTransformerType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_TransformerTypeCommon](../../psd/IfcElectricalDomain/Pset_TransformerTypeCommon.xml): property set for properties that are common to all types of transformer, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.