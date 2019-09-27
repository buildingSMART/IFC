﻿_IfcTypeProduct_ defines a type definition of a product without being already inserted into a project structure (without having a placement), and not being included in the geometric representation context of the project. It is used to define a product specification, that is, the specific product information that is common to all occurrences of that product type.

An _IfcTypeProduct_ may have a list of property set attached and an optional set of product representations. Values of these properties and the representation maps are common to all occurrences of that product type. The type-occurrence relationship is realized using the objectified relationship _IfcRelDefinesByType_.

> NOTE&nbsp; The product representations are defined as representation maps, which may be assigned by a product instance through the representation item(s) being an _IfcShapeRepresentation_ and having _Items_ of type _IfcMappedItem_.

The representations at the occurrence level (represented by subtypes of _IfcProduct_) can override the specific representations at the type level:

* for geometric representations, a Cartesian transformation operator can be applied at the occurrence level.
* for property sets, a property within an occurrence property set, assigned at the product occurrence, overrides the same property assigned to the product type.

An _IfcTypeProduct_ may be exchanged without being already assigned to subtypes of _IfcProduct_.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The entity _IfcTypeProduct_ shall not be instantiated from IFC4 onwards. It will be changed into an ABSTRACT supertype in future releases of IFC.
