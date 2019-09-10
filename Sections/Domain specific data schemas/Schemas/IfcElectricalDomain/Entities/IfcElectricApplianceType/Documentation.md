An _IfcElectricApplianceType_ defines a particular type of common electrical appliance found in a typical AEC/FM facility. Electrical Appliances generally consist of electrical devices that are not a fixed part of the building but instead can be moved from one space to another and are powered with electricity.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC R1.0.
Renamed from IfcElectricalFixture in IFC 2x. Renamed as
IfcElectricalApplianceType in IFC 2x2. </font>
> 


****Use Definitions****

An _IfcElectricApplianceType_ is a subtype of IfcFlowTerminalType that provides for various forms of electrical appliance.

Usage of _IfcElectricApplianceType_ defines the parameters for one or more occurrences of _IfcFlowTerminal_.

****Property Set Use Definition****:

The property sets relating to the _IfcElectricApplianceType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricApplianceType_ are part of this IFC release:

* [Pset_ElectricalDeviceCommon](../../psd/IfcElectricalDomain/Pset_ElectricalDeviceCommon.xml): property set for properties that are common to all types of electrical devices, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.
