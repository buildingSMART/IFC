The element type _IfcAirTerminalType_ defines a list of commonly shared property set definitions of an air terminal and an optional set of product representations. It is used to define an air terminal specification (i.e. the specific product information, that is common to all occurrences of that product type).

 
	 
	An air terminal is a terminating or origination point for the
    transfer of air between distribution system(s) and one or more spaces.
    It can also be used for the transfer of air between adjacent spaces.

	
> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A air terminal type is used to define the common properties of a air terminal that may be applied to many occurrences of that type. An air terminal is a mechanical device used to control the characteristics air at the entrance or exit to an open system, such as a room or space. Air terminal types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcAirTerminalType_ are represented by instances of _IfcFlowTerminal_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_AirTerminalTypeCommon](../../psd/IfcHvacDomain/Pset_AirTerminalTypeCommon.xml){ target="SOURCE"}: common property set for all air terminal types 
    * [Pset_AirTerminalTypeRectangular](../../psd/IfcHvacDomain/Pset_AirTerminalTypeRectangular.xml){ target="SOURCE"}: property set for rectangular shaped air terminal types 
    * [Pset_AirTerminalTypeRound](../../psd/IfcHvacDomain/Pset_AirTerminalTypeRound.xml){ target="SOURCE"}: property set for round shaped air terminal types 
    * [Pset_AirTerminalTypeSlot](../../psd/IfcHvacDomain/Pset_AirTerminalTypeSlot.xml){ target="SOURCE"}: property set for slot air terminal types 
    * [Pset_AirTerminalTypeSquare](../../psd/IfcHvacDomain/Pset_AirTerminalTypeSquare.xml){ target="SOURCE"}: property set for square shaped air terminal types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>