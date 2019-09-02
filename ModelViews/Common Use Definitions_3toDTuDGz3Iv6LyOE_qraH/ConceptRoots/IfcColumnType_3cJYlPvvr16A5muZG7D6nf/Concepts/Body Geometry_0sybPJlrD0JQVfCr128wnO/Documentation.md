The _IfcColumnType_ may define the shared geometric representation for all column occurrences. The _RepresentationMaps_ attribute refers to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShapeRepresentation_'s having an _RepresentationIdentifier_ 'Box', 'Axis', or 'Body'). It is only applicable if the _IfcColumnType_ has only occurrences of type _IfcColumn_ (See geometric use definition of _IfcColumn_ for further information).

> NOTE&nbsp; If the _IfcColumnType_ has an associated _IfcMaterialProfileSet_, then no shared geometric representation shall be provided.

> NOTE&nbsp; The product shape representations are defined as _RepresentationMaps_ (attribute of the supertype _IfcTypeProduct_), which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[n]_ being an _IfcMappedItem_. See _IfcTypeProduct_ for further information.

> NOTE&nbsp; The values of attributes _RepresentationIdentifier_ and _RepresentationType_ of _IfcShapeRepresentation_ are restricted in the same way as those for _IfcColumn_ and _IfcColumnStandardCase_