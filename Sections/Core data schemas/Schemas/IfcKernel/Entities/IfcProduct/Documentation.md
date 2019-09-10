Any object, or any aid to define, organize and annotate an object, that relates to a geometric or spatial context. Subtypes of _IfcProduct_ usually hold a shape representation and a local placement within the project structure.

This includes manufactured, supplied or created objects (referred to as elements) for incorporation into an AEC/FM project. This also includes objects that are created indirectly by other products, as spaces are defined by bounding elements. Products can be designated for permanent use or temporary use, an example for the latter is formwork. Products are defined by their properties and representations.

In addition to physical products (covered by the subtype _IfcElement_) and spatial items (covered by the subtype _IfcSpatialStructureElement_) the _IfcProduct_ also includes non-physical items, that relate to a geometric or spatial contexts, such as grid, port, annotation, structural actions, etc.

> <small><font color="#0000ff">HISTORY
New Entity in IFC Release 1.0</font></small>

**Use Definition**

Any instance of _IfcProduct_ defines a particular occurrence of a product, the common type information, that relates to many similar (or identical) occurrences of _IfcProduct_, is handled by the _IfcTypeProduct_ (and its subtypes), assigned to one or many occurrences of _IfcProduct_ by using the objectified relationship _IfcRelDefinesByType_. The _IfcTypeProduct_ may provide, in addition to common properties, also a common geometric representation for all occurrences.

An _IfcProduct_ occurs at a specific location in space if it has a geometric representation assigned. It can be placed relatively to other products, but ultimately relative to the world coordinate system defined for this project.

The inherited _ObjectType_ attribute can be used to designate a particular type of the product instance. If subtypes of _IfcProduct_ have a _PredefinedType_ defined, the _ObjectType_ is used to provide the user defined, particular type of the product instance, if the _PredefinedType_ is set to <font size="-1">USERDEFINED</font>.