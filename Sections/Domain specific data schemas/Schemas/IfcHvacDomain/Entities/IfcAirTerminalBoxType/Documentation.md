The element type _IfcAirTerminalBoxType_ defines a list of commonly shared property set definitions of an air termainal box and an optional set of product representations. It is used to define an air terminal box specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

An air terminal box type is used to define the common properties of an air terminal box that may be applied to many occurrences of that type. An air terminal box typically participates in an HVAC duct distribution system and is used to control or modulate the amount of air delivered to its downstream ductwork. Air terminal box types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcAirTerminalBoxType_ are represented by instances of _IfcFlowController_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_AirTerminalBoxTypeCommon](../../psd/IfcHvacDomain/Pset_AirTerminalBoxTypeCommon.xml){ target="SOURCE"}: common property set for all air terminal box types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
