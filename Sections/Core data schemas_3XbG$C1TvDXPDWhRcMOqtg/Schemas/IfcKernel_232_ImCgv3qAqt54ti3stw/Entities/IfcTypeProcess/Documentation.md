_IfcTypeProcess_ defines a specific (or type) definition of a process or activity without being assigned to a schedule or a time. It is used to define a process or activity specification, that is, the specific process or activity information that is common to all occurrences that are defined for that process or activity type.

An _IfcTypeProcess_ may have a list of property set attached. Values of these properties are common to all occurrences of that process or activity type. The type occurrence relationship is realized using the objectified relationship _IfcRelDefinesByType_.

Subtypes of _IfcTypeProcess_ may be exchanged without being already assigned to subtypes of _IfcProcess_.

> HISTORY&nbsp; New entity in IFC4.

{ .use-head}
Property set use definition

An _IfcTypeProcess_ may have a list of property sets attached, accessible by the attribute _SELF\IfcTypeObject.HasPropertySets_. Currently there are no predefined property sets defined as part of the IFC specification.

> NOTE&nbsp; For property sets, a property within an occurrence property set that is assigned at the process occurrence, overrides the same property assigned to the process type.