The element type _IfcEvaporatorType_ defines a list of commonly shared property set definitions of an evaporator and an optional set of product representations. It is used to define an evaporator specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A evaporator type is used to define the common properties of an evaporator that may be applied to many occurrences of that type. An evaporator is a device in which a liquid refrigerent is vaporized and absorbs heat from the surrounding fluid. Evaporator types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcEvaporatorType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_EvaporatorTypeCommon](../../psd/IfcHvacDomain/Pset_EvaporatorTypeCommon.xml){ target="SOURCE"}: common property set for all evaporator types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>