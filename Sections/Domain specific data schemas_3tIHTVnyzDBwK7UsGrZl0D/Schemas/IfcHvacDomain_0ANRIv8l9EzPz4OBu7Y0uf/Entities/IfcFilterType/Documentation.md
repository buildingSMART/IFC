The element type _IfcFilterType_ defines a list of commonly shared property set definitions of a filter and an optional set of product representations. It is used to define a filter specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A filter type is used to define the common properties of a filter that may be applied to many occurrences of that type. A filter is an apparatus used to remove particulate or gaseous matter from fluids and gases. Filter types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFilterType_ are represented by instances of _IfcTreatmentDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_FilterTypeCommon](../../psd/IfcHvacDomain/Pset_FilterTypeCommon.xml){ target="SOURCE"}: common property set for all filter types 
    * [Pset_FilterTypeAirParticleFilter](../../psd/IfcHvacDomain/Pset_FilterTypeAirParticleFilter.xml){ target="SOURCE"}: property set for all air particle filter types 


> <font size="-1">
    	NOTE: This entity has been renamed from <i>IfcAirFilter</i> in 
        IFC R2x.
    	</font>

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>