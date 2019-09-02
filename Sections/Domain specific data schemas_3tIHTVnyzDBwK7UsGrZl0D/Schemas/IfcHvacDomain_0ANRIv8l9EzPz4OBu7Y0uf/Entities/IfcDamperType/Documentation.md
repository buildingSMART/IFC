The element type _IfcDamperType_ defines a list of commonly shared property set definitions of a damper and an optional set of product representations. It is used to define a damper specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A damper type is used to define the common properties of a damper that may be applied to many occurrences of that type. A damper typically participates in an HVAC duct distribution system and is used to control or modulate the flow of air. Damper types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcDamperType_ are represented by instances of _IfcFlowController_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DamperTypeCommon](../../psd/IfcHvacDomain/Pset_DamperTypeCommon.xml){ target="SOURCE"}: common property set for all damper types 
    * [Pset_DamperTypeControlDamper](../../psd/IfcHvacDomain/Pset_DamperTypeControlDamper.xml){ target="SOURCE"}: property set for all control damper types 
    * [Pset_DamperTypeFireDamper](../../psd/IfcHvacDomain/Pset_DamperTypeFireDamper.xml){ target="SOURCE"}: property set for all fire damper types 
    * [Pset_DamperTypeFireSmokeDamper](../../psd/IfcHvacDomain/Pset_DamperTypeFireSmokeDamper.xml){ target="SOURCE"}: property set for all combination fire and smoke damper types 
    * [Pset_DamperTypeSmokeDamper](../../psd/IfcHvacDomain/Pset_DamperTypeSmokeDamper.xml){ target="SOURCE"}: property set for all smoke damper types  

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>