The objectified relationship _IfcRelDefinesByTemplate_ defines the relationships between property set template and property sets. Common information about property sets, e.g. the applicable name, description, contained properties, is defined by the property set template and assigned to all property sets.

> NOTE&nbsp; The assignment of an _IfcPropertySetTemplate_ is supported for _IfcPropertySet_ and _IfcQuantitySet_.

The _IfcRelDefinesByTemplate_ is a 1-to-N relationship, as it allows for the assignment of one property set template to a single or to many property sets or quantity sets. Those property sets then share the same property set template definition.

> HISTORY&nbsp; New entity in IFC4.