The element type _IfcCooledBeamType_ defines a list of commonly shared property set definitions of a cooled beam and an optional set of product representations. It is used to define a cooled beam specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A cooled beam type is used to define the common properties of a cooled beam that may be applied to many occurrences of that type. A cooled beam is a device typically used to cool air by circulating a fluid such as chilled water through exposed finned tubes above a space. Cooled beam types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCooledBeamType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_CooledBeamTypeCommon](../../psd/IfcHvacDomain/Pset_CooledBeamTypeCommon.xml){ target="SOURCE"}: common property set for all cooled beam types 
    * [Pset_CooledBeamTypeActive](../../psd/IfcHvacDomain/Pset_CooledBeamTypeActive.xml){ target="SOURCE"}: property set for all active or ventilated cooled beam types  

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>