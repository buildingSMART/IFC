An _IfcCableSegmentType_ is a type of flow segment used to carry electrical power or communications signals.

> <font color="#0000ff" size="-1">
HISTORY: New entity
in IFC 2x2.</font>

****Use Definitions****

A cable segment type is used to define the common properties of a cable segment that may be applied to many occurrences of that type. A cable segment is used to typically join two sections of an electrical network or a network of components carrying the electrical service. Cable segment types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCableSegmentType_ are represented by instances of _IfcFlowSegment_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to the _IfcCableSegmentType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcCableSegmentType_are part of this IFC release:

* [Pset_CableSegmentTypeCableSegment](../../psd/IfcElectricalDomain/Pset_CableSegmentTypeCableSegment.xml): specific property set for the properties of a whole cable (including the aggregation of conductors within the cable), if available 
* [Pset_CableSegmentTypeConductorSegment](../../psd/IfcElectricalDomain/Pset_CableSegmentTypeConductorSegment.xml): specific property set for the properties of an individual conductor within an electrical cable, if available.

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.