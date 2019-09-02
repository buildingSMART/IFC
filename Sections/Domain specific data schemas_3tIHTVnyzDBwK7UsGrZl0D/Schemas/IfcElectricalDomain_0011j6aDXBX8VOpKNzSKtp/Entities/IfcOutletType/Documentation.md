An _IfcOutletType_ defines a particular type of outlet which is a device installed at a point to receive an inserted plug.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2 </font>
> 


****Use Definitions****

An _IfcOutletType_ provides for all forms of outlet.

Usage of _IfcOutletType_ defines the parameters for one or more occurrences of _IfcFlowTerminal_. Parameters are specified through property sets that are enumerated in the _IfcOutletTypeEnum_ data type.

****Property Set Use Definition****:

The property sets relating to the _IfcProtectiveDeviceType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcProtectiveDeviceType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 
* [Pset_OutletTypeCommon](../../psd/IfcElectricalDomain/Pset_OutletTypeCommon.xml): property set for properties that are common to all types of cabled outlet, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.