The element type _IfcTransportElementType_ defines commonly shared information for occurrences of transport elements. The set of shared information may include:

* common properties within shared property sets
* common material information
* common shape representations

It is used to define a transport element specification (i.e. the specific product information that is common to all occurrences of that beam type). Transport element types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcTransportElementType_ are represented by instances of _IfcTransportElement_ (or its subtypes).

> HISTORY&nbsp; New entity in IFC2x2.

{ .use-head}
Geometry Use Definition

The _IfcTransportElementType_ may define the shared geometric representation for all transport element occurrences. The _RepresentationMaps_ attribute refers to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShaperepresentation_'s having an _RepresentationIdentifier_ 'Box', 'FootPrint', or 'Body').

> NOTE&nbsp; The product shape representations are defined as _RepresentationMaps_ (attribute of the supertype _IfcTypeProduct_), which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[n]_ being an _IfcMappedItem_. See _IfcTypeProduct_ for further information.

> NOTE&nbsp; The values of attributes _RepresentationIdentifier_ and _RepresentationType_ of _IfcShapeRepresentation_ are restricted in the same way as those for _IfcTransportElementType_.
