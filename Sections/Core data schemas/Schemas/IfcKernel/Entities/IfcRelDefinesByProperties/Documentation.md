﻿The objectified relationship _IfcRelDefinesByProperties_ defines the relationships between property set definitions and objects. Properties are aggregated in property sets. Property sets can be either directly assigned to occurrence objects using this relationship, or assigned to an object type and assigned via that type to occurrence objects. The assignment of an _IfcPropertySet_ to an _IfcTypeObject_ is not handled via this objectified relationship, but through the direct relationship _HasPropertySets_ at _IfcTypeObject_.

The _IfcRelDefinesByProperties_ is an N-to-N relationship, as it allows for the assignment of one or more property sets to one or more objects. Those objects then share the same property definition.

> HISTORY&nbsp; New entity in IFC2.0. Has been renamed from _IfcRelAssignsProperties_ in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The attribute _RelatedObjects_ had been demoted from the supertype _IfcRelDefines_ to _IfcRelDefinesByProperties_. This relationship has been modified to support multiple property sets referenced by a single relationship.
