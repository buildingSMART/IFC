An _IfcConstructionProductResource_ defines the role of a product that is consumed (wholly or partially), or occupied (i.e. used) in the performance of construction.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Renamed from IfcProductResource in IFC 2x.</font>

### Use Definition
Occurrences of products that are used as product resources are instances of _IfcProduct_ (by reference) since they result from some processes. For instance, formworks can be instantiated as products resulting from the process &#145;constructing formwork&#146;. However, they are used as resources in the process &#145;pouring concrete&#146; in a later stage of the project. The product that is used as a construction resource is referenced using the _IfcRelAssignsToResource.RelatedObjects_ relationship.