The objectified relationship _IfcRelDefinesByProperties_ defines the relationships between property set definitions and objects. Properties are aggregated in property sets. Property sets can be either directly assigned to occurrence objects using this relationship, or assigned to an object type and assigned via that type to occurrence objects.

The _IfcRelDefinesByProperties_ is a 1-to-N relationship, as it allows for the assignment of one property set to a single or to many objects. Those objects then share the same property definition.

> HISTORY&nbsp; New entity in IFC2.0. Has been renamed from _IfcRelAssignsProperties_ in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _RelatedObjects_ had been demoted from the supertype _IfcRelDefines_ to _IfcRelDefinesByProperties_.
