The element type _IfcEnergyConversionType_ defines a list of commonly shared property set definitions of an energy conversion device and an optional set of product representations. It is used to define an energy conversion device specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A energy conversion type is used to define the common properties of a energy conversion device that may be applied to many occurrences of that type. An energy conversion device is a building systems device that converts energy from one form into another such as a boiler (i.e., combusting gas to heat water), chiller (i.e., using a refrigeration cycle to cool a liquid), or a cooling coil (i.e., using the phase-change characteristics of a refrigerant to cool air). Energy conversion types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcEnergyConversionType_ are represented by instances of _IfcEnergyConversion_ or its subtypes.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>