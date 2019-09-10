The element type _IfcSpaceHeaterType_ defines a list of commonly shared property set definitions of a space heater and an optional set of product representations. It is used to define a space heater specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
    	NOTE: This entity subsumes the entities <i>IfcHydronicHeater</i> and
        <i>IfcUnitHeater</i> from IFC R2x.
    	</font>

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A space heater type is used to define the common properties of a space heater device that may be applied to many occurrences of that type. Space heaters utilize a combination of radiation and/or natural convection using a heating source such as steam or hot water. Examples of space heaters include radiators, convectors, baseboard and finned-tube heaters, etc. Space heater types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcSpaceHeaterType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_SpaceHeaterTypeCommon](../../psd/IfcHvacDomain/Pset_SpaceHeaterTypeCommon.xml){ target="SOURCE"}: common property set for all space heater types 
    * [Pset_SpaceHeaterTypeHydronic](../../psd/IfcHvacDomain/Pset_SpaceHeaterTypeHydronic.xml){ target="SOURCE"}: property set for all hydronic space heater types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>