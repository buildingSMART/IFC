The element type _IfcGasTerminalType_ defines a list of commonly shared property set definitions of a gas terminal and an optional set of product representations. It is used to define a gas terminal specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A gas terminal type is used to define the common properties of a gas terminal that may be applied to many occurrences of that type. A gas terminal is a device where gas is consumed or combusted, such as in a gas-fired hot water or steam boiler. Gas terminal types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcGasTerminalType_ are represented by instances of _IfcFlowTerminal_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_GasTerminalTypeCommon](../../psd/IfcHvacDomain/Pset_GasTerminalTypeCommon.xml){ target="SOURCE"}: common property set for all gas terminal types 
    * [Pset_GasTerminalTypeGasAppliance](../../psd/IfcHvacDomain/Pset_GasTerminalTypeGasAppliance.xml){ target="SOURCE"}: property set for all gas appliance terminal types 

    * [Pset_GasTerminalTypeGasBurner](../../psd/IfcHvacDomain/Pset_GasTerminalTypeGasBurner.xml){ target="SOURCE"}: property set for all gas burner terminal types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>