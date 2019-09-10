The element type _IfcFanType_ defines a list of commonly shared property set definitions of a fan and an optional set of product representations. It is used to define a fan specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A Fan type is used to define the common properties of a fan that may be applied to many occurrences of that type. A fan is a device which imparts mechanical work on a gas. A typical usage of a fan is to induce airflow in a building services air distribution system. Fan types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFanType_ are represented by instances of _IfcFlowMovingDevice_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_FanTypeCommon](../../psd/IfcHvacDomain/Pset_FanTypeCommon.xml){ target="SOURCE"}: common property set for all fan types 
    * [Pset_FanTypeSmokeControl](../../psd/IfcHvacDomain/Pset_FanTypeSmokeControl.xml){ target="SOURCE"}: property set for all fan types that are part of a smoke control system 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>