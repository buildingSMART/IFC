The element type _IfcTubeBundleType_ defines a list of commonly shared property set definitions of a tube buncle and an optional set of product representations. It is used to define a tube bundle specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A tube bundle type is used to define the common properties of a tube bundle that may be applied to many occurrences of that type. A tube bundle is a device consisting of tubes and bundles of tubes used for heat transfer and contained typically within other energy conversion devices, such as a chiller or coil.

The occurrences of the _IfcTubeBundleType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_TubeBundleTypeCommon](../../psd/IfcHvacDomain/Pset_TubeBundleTypeCommon.xml){ target="SOURCE"}: common property set for all tube bundle types 
    * [Pset_TubeBundleTypeFinned](../../psd/IfcHvacDomain/Pset_TubeBundleTypeFinned.xml){ target="SOURCE"}: property set for finned tube bundle types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
