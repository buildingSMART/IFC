The objectified relationship (_IfcRelAssociatesDocument_) handles the assignment of a document information (items of the select _IfcDocumentSelect_) to objects occurrences (subtypes of _IfcObject_) or object types (subtypes of _IfcTypeObject_).

The relationship is used to assign a document reference or a more detailed document information to objects. A single document reference can be applied to multiple objects.

The inherited attribute _RelatedObjects_ define the objects to which the document association is applied. The attribute _RelatingDocument_ is the reference to a document reference, applied to the object(s).

> HISTORY&nbsp; New entity in IFC2x.