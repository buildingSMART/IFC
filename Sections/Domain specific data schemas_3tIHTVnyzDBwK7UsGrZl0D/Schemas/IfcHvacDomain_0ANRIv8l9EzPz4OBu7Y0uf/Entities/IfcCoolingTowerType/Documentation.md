The element type _IfcCoolingTowerType_ defines a list of commonly shared property set definitions of a cooling tower and an optional set of product representations. It is used to define a cooling tower specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A cooling tower type is used to define the common properties of a cooling tower that may be applied to many occurrences of that type. A cooling tower is a device which rejects heat to ambient air by circulating a fluid such as water through it to reduce its temperature by partial evaporation. Cooling tower types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCoolingTowerType_ are represented by instances of _IfcEnergyConversionDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_CoolingTowerTypeCommon](../../psd/IfcHvacDomain/Pset_CoolingTowerTypeCommon.xml){ target="SOURCE"}: common property set for all cooling tower types 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>