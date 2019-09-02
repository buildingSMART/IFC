The _IfcElementAssemblyType_ defines a list of commonly shared property set definitions of an element and an optional set of product representations. It is used to define an element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

An element assembly type is used to define the common properties of a certain type of an element assembly that may be applied to many instances of that type to assign a specific style. An element assembly types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcElementAssemblyType_ are represented by instances of _IfcElementAssembly_.

> HISTORY&nbsp; New entity in IFC4.