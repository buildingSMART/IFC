A space represents an area or volume bounded actually or theoretically. Spaces are areas or volumes that provide for certain functions within a building.

The _IfcSpaceType_ defines a list of commonly shared defines commonly shared information for occurrences of spaces. The set of shared information may include:

* common properties within shared property sets 
* common shape representations 

It is used to define an space specification (i.e. the specific space information, that is common to all occurrences of that space type. Space types may be exchanged without being already assigned to occurrences.

> NOTE&nbsp; The space types are often used to represent space catalogues, less so for sharing a common representation map. Space types in a space catalogue share same space classification and a common set of space requirement properties.

The occurrences of _IfcSpaceType_ are represented by instances of _IfcSpace_.

> HISTORY&nbsp; New entity in IFC2x3.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _LongName_ has been added to the end of the entity definition.

{ .use-head}
Geometry Use Definition

The _IfcSpaceType_ may define the shared geometric representation for all space occurrences. The _RepresentationMaps_ attribute refers to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShaperepresentation_'s having an RepresentationIdentifier 'Box', 'FootPrint', or 'Body').

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_. However view definitions and implementer agreements may prevent the usage of shared geometry for spaces.