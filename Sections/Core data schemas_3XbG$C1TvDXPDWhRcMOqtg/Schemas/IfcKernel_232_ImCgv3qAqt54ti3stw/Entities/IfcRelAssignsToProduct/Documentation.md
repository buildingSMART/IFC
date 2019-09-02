The objectified relationship _IfcRelAssignsToProduct_ handles the assignment of objects (subtypes of _IfcObject_) to a product (subtypes of _IfcProduct_). The _Name_ attribute should be used to classify the usage of the _IfcRelAssignsToProduct_ objectified relationship. The following _Name_ values are proposed:

* 'Context' : Assignment of a context specific representation, such as of structural members to a different context representation (with potentially different decomposition breakdown) such as of building elements for a specific context specific representation. 
* 'View' : Assignment of a product (via _RelatingProduct_) that is decomposed according to a discipline view, to another product (via _RelatedObjects_) that is decomposed according to a different discipline view. An example is the assignment of the architectural slab to a different decomposition of the pre manufactured sections of a slab (under a precast concrete discipline view).

> HISTORY&nbsp; New entity in IFC2x

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The reference of a product within a spatial structure is now handled by a new relationship object _IfcRelReferencedInSpatialStructure_. The _IfcRelAssignsToProduct_ shall not be used to represent this relation from IFC2x3 onwards.