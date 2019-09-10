_IfcTypeResource_ defines a specific (or type) definition of a resource. It is used to define a resource specification (the specific resource, that is common to all occurrences that are defined for that resource) and could act as a resource template.

An _IfcTypeResource_ may have a list of property sets attached. Values of these properties are common to all occurrences of that resource type. The type occurrence relationship is realized using the objectified relationship _IfcRelDefinesByType_.

Subtypes of _IfcTypeResource_ may be exchanged without being already assigned to subtypes of _IfcResource_.

> HISTORY&nbsp; New entity in IFC4.

{ .use-head}
Property set use definition

An _IfcTypeResource_ may have a list of property sets attached, accessible by the attribute _SELF\IfcTypeObject.HasPropertySets_. Currently there are no predefined property sets defined as part of the IFC specification.

> NOTE&nbsp; For property sets, a property within an occurrence property set that is assigned at the resource occurrence, overrides the same property assigned to the resource type.