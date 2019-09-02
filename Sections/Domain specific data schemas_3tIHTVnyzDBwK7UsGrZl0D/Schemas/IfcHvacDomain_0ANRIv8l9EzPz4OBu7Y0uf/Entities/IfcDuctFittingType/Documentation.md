The element type _IfcDuctFittingType_ defines a list of commonly shared property set definitions of a duct fitting and an optional set of product representations. It is used to define an duct fitting specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A Duct fitting type is used to define the common properties of a duct fitting that may be applied to many occurrences of that type. A duct fitting is a junction or transition in a flow distribution system (e.g., elbow, tee, etc.). Duct fitting types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcDuctFittingType_ are represented by instances of _IfcFlowFitting_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DuctFittingTypeCommon](../../psd/IfcHvacDomain/Pset_DuctFittingTypeCommon.xml){ target="SOURCE"}: common property set for all duct fitting types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>