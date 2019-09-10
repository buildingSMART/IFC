The _IfcBuildingElementType_ provides the type information for _IfcBuildingElement_ occurrences.

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

A building element type is used to define the common properties of a certain type of building element that are applied to all occurrences of that type. It is used to define a building element specification (i.e. the specific product information, that is common to all occurrences of that product type). Building element types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The _IfcBuildingElementType_ is an abstract type that cannot be instantiated. For arbitrary building element types, that cannot be expressed by a subtype of _IfcBuildingElementType_, use _IfcBuildingElementProxyType_. Occurrences of subtypes of the _IfcBuildingElementType_ are represented by instances of the appropriate subtypes of _IfcBuildingElement_.

> HISTORY&nbsp; New entity in IFC2x2.
