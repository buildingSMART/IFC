The element type _IfcChillerType_ defines a list of commonly shared property set definitions of a chiller and an optional set of product representations. It is used to define a chiller specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A chiller type is used to define the common properties of a chiller that may be applied to many occurrences of that type. A chiller is a device used to implement a refrigeration cycle for cooling a fluid, typically water or a mixture of water and glycol. The chilled water is then used to cool and dehumidify air in a building. Chiller types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcChillerType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_ChillerTypeCommon](../../psd/IfcHvacDomain/Pset_ChillerTypeCommon.xml){ target="SOURCE"}: common property set for all chiller types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
