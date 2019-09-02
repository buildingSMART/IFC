_IfcSanitaryTerminalType_ defines a particular type of _IfcFlowTerminal_ that is a fixed appliance or terminal usually supplied with water and used for drinking, cleaning or foul water disposal or that is an item of equipment directly used with such an appliance or terminal.

Refer also to definition in BS6100 100 3406.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x Edition 2.</font>
> 


****Use Definitions****

The _IfcSanitaryTerminalType_ defines a particular type of sanitary terminal, which may be included into the spatial context of the building model through an (or multiple) instances of _IfcFlowTerminal_.

The parameters of the sanitary terminal type are defined through the type driven property sets referred to by the predefined type attribute of _IfcSanitaryTerminalType_.

****Property Set Use Definition****:

The property sets relating to the _IfcSanitaryTerminalType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcSanitaryTerminalType_ are part of this IFC release:

* [Pset_SanitaryTerminalTypeBath](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeBath.xml): specific property set for the properties of a bath , if available 
* [Pset_SanitaryTerminalTypeBidet](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeBidet.xml): specific property set for the properties of a bidet , if available 
* [Pset_SanitaryTerminalTypeCistern](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeCistern.xml): specific property set for the properties of a cistern (associated with a WC, urinal or range of such devices), if available 
* [Pset_SanitaryTerminalTypeSanitaryFountain](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeSanitaryFountain.xml): specific property set for the properties of a sanitary fountain, typically for drinking water, if available
* [Pset_SanitaryTerminalTypeShower](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeShower.xml): specific property set for the properties of a shower, if available
* [Pset_SanitaryTerminalTypeSink](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeSink.xml): specific property set for the properties of a sink , if available 
* [Pset_SanitaryTerminalTypeToiletPan](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeToiletPan.xml): specific property set for the properties of a toilet pan, if available 
* [Pset_SanitaryTerminalTypeUrinal](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeUrinal.xml): specific property set for the properties of a urinal, if available 
* [Pset_SanitaryTerminalTypeWCSeat](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeWCSeat.xml): specific property set for the properties of a WC seat, if available
* [Pset_SanitaryTerminalTypeWashHandBasin](../../psd/IfcPlumbingFireProtectionDomain/Pset_SanitaryTerminalTypeWashHandBasin.xml): specific property set for the properties of a wash hand basin, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.