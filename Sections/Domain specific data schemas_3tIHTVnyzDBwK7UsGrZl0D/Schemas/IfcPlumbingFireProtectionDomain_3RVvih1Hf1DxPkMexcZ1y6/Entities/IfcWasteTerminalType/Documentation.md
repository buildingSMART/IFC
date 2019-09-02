The _IfcWasteTerminalType_ defines a particular type of sanitary flow that has the purpose of collecting or intercepting waste from one or more sanitary terminals or other fluid waste generating equipment and discharging it into a single waste/drainage system.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcWasteTerminalType_ provides for all forms of trap, waste point and interceptor that collects discharge from a sanitary terminal and discharges it into a waste/drainage subsystem or that collects waste from several terminals and passes it into a single waste/drainage subsystem. This includes the P and S traps from soil sanitary terminals, sinks, basins etc. as well as floor wastes, gully traps and interceptors that provide collection points.

An _IfcWasteTerminalType_ may be included into the spatial context of the building model through an (or multiple) instances of _IfcFlowTerminal_.

The parameters of the waste terminal type are defined through the type driven property sets referred to by the predefined type attribute of _IfcWasteTerminalType_.

****Property Set Use Definition****:

The property sets relating to the _IfcWasteTerminalType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcWasteTerminalType_ are part of this IFC release:

* [Pset_WasteTerminalTypeFloorTrap](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeFloorTrap.xml): specific property set for the properties of a floor trap, if available 
* [Pset_WasteTerminalTypeFloorWaste](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeFloorWaste.xml): specific property set for the properties of a floor waste unit, if available 
* [Pset_WasteTerminalTypeGreaseInterceptor](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeGreaseInterceptor.xml): specific property set for the properties of a grease interceptor, if available 
* [Pset_WasteTerminalTypeGullySump](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeGullySump.xml): specific property set for the properties of a gully sump, if available
* [Pset_WasteTerminalTypeGullyTrap](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeGullyTrap.xml): specific property set for the properties of a gully trap, if available
* [Pset_WasteTerminalTypeOilInterceptor](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeOilInterceptor.xml): specific property set for the properties of an oil interceptor, if available 
* [Pset_WasteTerminalTypePetrolInterceptor](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypePetrolInterceptor.xml): specific property set for the properties of a petrol interceptor, if available 
* [Pset_WasteTerminalTypeRoofDrain](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeRoofDrain.xml): specific property set for the properties of a roof drain, if available 
* [Pset_WasteTerminalTypeWasteDisposalUnit](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeWasteDisposalUnit.xml): specific property set for the properties of a waste disposal unit, if available
* [Pset_WasteTerminalTypeWasteTrap](../../psd/IfcPlumbingFireProtectionDomain/Pset_WasteTerminalTypeWasteTrap.xml): specific property set for the properties of a waste trap, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.