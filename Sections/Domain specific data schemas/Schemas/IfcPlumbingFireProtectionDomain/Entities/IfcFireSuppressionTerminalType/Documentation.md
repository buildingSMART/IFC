The _IfcFireSuppressionTerminalType_ defines a particular type of _IfcFlowTerminal_ that has the purpose of delivering a fluid (gas or liquid) that will suppress a fire.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcFireSuppressionTerminalType_ provides for all forms of sprinkler, spreader and other form of terminal that is connected to a pipework system and intended to act in the role of suppressing a fire .

An _IfcFireSuppressionTerminalType_ may be included into the spatial context of the building model through an (or multiple) instances of _IfcFlowTerminal_.

The parameters of the fire suppression terminal type are defined through the type driven property sets referred to by the predefined type attribute of _IfcFireSuppressionTerminalType_.

****Property Set Use Definition****:

The property sets relating to the _IfcFireSuppressionTerminalType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcFireSuppressionTerminalType_ are part of this IFC release:

* [Pset_FireSuppressionTerminalTypeBreechingInlet](../../psd/IfcPlumbingFireProtectionDomain/Pset_FireSuppressionTerminalTypeBreechingInlet.xml): specific property set for the properties of a breeching inlet, if available
* [Pset_FireSuppressionTerminalTypeFireHydrant](../../psd/IfcPlumbingFireProtectionDomain/Pset_FireSuppressionTerminalTypeFireHydrant.xml): specific property set for the properties of a fire hydrant, if available 
* [Pset_FireSuppressionTerminalTypeSprinkler](../../psd/IfcPlumbingFireProtectionDomain/Pset_FireSuppressionTerminalTypeSprinkler.xml): specific property set for the properties of a sprinkler, if available 
* [Pset_FireSuppressionTerminalTypeHoseReel](../../psd/IfcPlumbingFireProtectionDomain/Pset_FireSuppressionTerminalTypeHoseReel.xml): specific property set for the properties of a hose reel, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.