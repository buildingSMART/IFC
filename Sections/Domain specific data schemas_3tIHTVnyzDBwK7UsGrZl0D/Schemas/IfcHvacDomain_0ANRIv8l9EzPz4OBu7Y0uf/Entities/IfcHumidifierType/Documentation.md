The element type _IfcHumidifierType_ defines a list of commonly shared property set definitions of a humidifier and an optional set of product representations. It is used to define a humidifier specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A Humidifier type is used to define the common properties of a humidifier that may be applied to many occurrences of that type. A humidifier is a device that adds moisture into the air. Humidifier types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcHumidifierType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_HumidifierTypeCommon](../../psd/IfcHvacDomain/Pset_HumidifierTypeCommon.xml){ target="SOURCE"}: common property set for all humidifier types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>