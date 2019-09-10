The element type _IfcCoilType_ defines a list of commonly shared property set definitions of a coil and an optional set of product representations. It is used to define a coil specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A coil type is used to define the common properties of a coil that may be applied to many occurrences of that type. A coil is a device used to provide heat transfer between non-mixing media. A common example is a cooling coil, which utilizes a finned coil in which circulates chilled water, antifreeze, or refrigerant that is used to remove heat from air moving across the surface of the coil. Coil types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCoilType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_CoilTypeCommon](../../psd/IfcHvacDomain/Pset_CoilTypeCommon.xml){ target="SOURCE"}: common property set for all coil types 
    * [Pset_CoilTypeHydronic](../../psd/IfcHvacDomain/Pset_CoilTypeHydronic.xml){ target="SOURCE"}: property set for hydronic coil types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
