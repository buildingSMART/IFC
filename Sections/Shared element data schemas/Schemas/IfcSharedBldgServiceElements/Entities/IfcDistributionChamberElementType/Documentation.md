The element type _IfcDistributionChamberElementType_ defines a list of commonly shared property set definitions of a distribution chamber element and an optional set of product representations. It is used to define a distribution chamber element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A distribution chamber element type is used to define the common properties of a distribution chamber element that may be applied to many occurrences of that type. A distribution chamber element is a formed volume used in a distribution system, such as a sump, trench or manhole. Distribution chamber element types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcDistributionChamberElementType_ are represented by instances of _IfcDistributionElement_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

    * [Pset_DistributionChamberElementTypeFormedDuct](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeFormedDuct.xml){ target="SOURCE"}: property set for formed duct distribution chamber element types 
    * [Pset_DistributionChamberElementTypeInspectionChamber](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeInspectionChamber.xml){ target="SOURCE"}: property set for inspection chamber distribution chamber element types 
    * [Pset_DistributionChamberElementTypeInspectionPit](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeInspectionPit.xml){ target="SOURCE"}: property set for inspection pit distribution chamber element types 
    * [Pset_DistributionChamberElementTypeManhole](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeManhole.xml){ target="SOURCE"}: property set for manhole distribution chamber element types 
    * [Pset_DistributionChamberElementTypeMeterChamber](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeMeterChamber.xml){ target="SOURCE"}: property set for meter chamber distribution chamber element types 
    * [Pset_DistributionChamberElementTypeSump](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeSump.xml){ target="SOURCE"}: property set for sump distribution chamber element types 
    * [Pset_DistributionChamberElementTypeTrench](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeTrench.xml){ target="SOURCE"}: property set for trench distribution chamber element types 
    * [Pset_DistributionChamberElementTypeValveChamber](../../psd/IfcSharedBldgServiceElements/Pset_DistributionChamberElementTypeValveChamber.xml){ target="SOURCE"}: property set for valve chamber distribution chamber element types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
