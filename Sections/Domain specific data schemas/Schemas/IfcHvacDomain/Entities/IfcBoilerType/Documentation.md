The element type _IfcBoilerType_ defines a list of commonly shared property set definitions of a boiler and an optional set of product representations. It is used to define a boiler specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A boiler type is used to define the common properties of a boiler that may be applied to many occurrences of that type. A boiler is a device which converts stored energy to heat which is added to a fluid; typically used to heat water. Boiler types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcBoilerType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_BoilerTypeCommon](../../psd/IfcHvacDomain/Pset_BoilerTypeCommon.xml){ target="SOURCE"}: common property set for all boiler types 
    * [Pset_BoilerTypeSteam](../../psd/IfcHvacDomain/Pset_BoilerTypeSteam.xml){ target="SOURCE"}: property set for steam boiler types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
