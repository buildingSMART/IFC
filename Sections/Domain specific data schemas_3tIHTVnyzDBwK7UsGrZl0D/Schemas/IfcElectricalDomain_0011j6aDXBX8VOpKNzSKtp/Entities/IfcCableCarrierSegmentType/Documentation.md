The _IfcCableCarrierSegmentType_ is a flow segment that is specifically used to carry and support cabling.

> <font color="#0000ff" size="-1">
HISTORY: New entity
in IFC 2x2.</font>

****Use Definitions****

An _IfcCableCarrierSegmentType_ is used to define the common properties of a cable carrier segment that may be applied to many occurrences of that type. A cable carrier segment is used to carry and supports components of a cabling system. Cable carrier segment types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCableCarrierSegmentType_ are represented by instances of _IfcFlowSegment_ or its subtypes.

****Property Set Use Definition:****

The property sets relating to the IfcCableCarrierSegmentType are defined by the IfcPropertySet and attached by the IfcRelDefinesByType relationship. It is accessible by the inverse IsDefinedBy relationship. The following property set definitions specific to the IfcCableCarrierSegmentType are part of this IFC release:

* [Pset_CableCarrierSegmentTypeCableLadderSegment](../../psd/IfcElectricalDomain/Pset_CableCarrierSegmentTypeCableLadderSegment.xml): specific property set for the properties of a segment of a cable ladder, if available 
* [Pset_CableCarrierSegmentTypeCableTraySegment](../../psd/IfcElectricalDomain/Pset_CableCarrierSegmentTypeCableTraySegment.xml): specific property set for the properties of a segment of cable tray, if available
* [Pset_CableCarrierSegmentTypeCableTrunkingSegment](../../psd/IfcElectricalDomain/Pset_CableCarrierSegmentTypeCableTrunkingSegment.xml): specific property set for the properties of a segment of cable trunking, if available
* [Pset_CableCarrierSegmentTypeConduitSegment](../../psd/IfcElectricalDomain/Pset_CableCarrierSegmentTypeConduitSegment.xml): : specific property set for the properties of a segment of electrical conduit, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.