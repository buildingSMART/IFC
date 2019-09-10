The element type _IfcUnitaryEquipmentType_ defines a list of commonly shared property set definitions of a unitary equipment element and an optional set of product representations. It is used to define a unitary equipment element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A unitary equipment type is used to define the common properties of unitary equipment that may be applied to many occurrences of that type. Unitary equipment typically combine a number of components into a single product, such as pre-packaged rooftop air-conditioning units, split systems, etc. Unitary equipment types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcUnitaryEquipmentType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

    * [Pset_UnitaryEquipmentTypeAirConditioningUnit](../../psd/IfcHvacDomain/Pset_UnitaryEquipmentTypeAirConditioningUnit.xml){ target="SOURCE"}: property set for air conditioning unitary equipment types 

    * [Pset_UnitaryEquipmentTypeAirHandler](../../psd/IfcHvacDomain/Pset_UnitaryEquipmentTypeAirHandler.xml){ target="SOURCE"}: property set for air handling unitary equipment types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
