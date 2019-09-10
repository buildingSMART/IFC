The element type _IfcTankType_ defines a list of commonly shared property set definitions of a tank and an optional set of product representations. It is used to define a tank specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A tank type is used to define the common properties of a Tank that may be applied to many occurrences of that type. A tank is a device used to hold gasses and liquids. Tank types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcTankType_ are represented by instances of _IfcFlowStorageDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_TankTypeCommon](../../psd/IfcHvacDomain/Pset_TankTypeCommon.xml){ target="SOURCE"}: common property set for all tank types 
    * [Pset_TankTypeExpansion](../../psd/IfcHvacDomain/Pset_TankTypeExpansion.xml){ target="SOURCE"}: property set for expansion tank types 

    * [Pset_TankTypePreformed](../../psd/IfcHvacDomain/Pset_TankTypePreformed.xml){ target="SOURCE"}: property set for preformed tank types 

    * [Pset_TankTypePressureVessel](../../psd/IfcHvacDomain/Pset_TankTypePressureVessel.xml){ target="SOURCE"}: property set for pressure vessel tank types 

    * [Pset_TankTypeSectional](../../psd/IfcHvacDomain/Pset_TankTypeSectional.xml){ target="SOURCE"}: property set for sectional tank types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
