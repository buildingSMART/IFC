The element type (_IfcBuildingElementType_) defines a list of commonly shared property set definitions of a building element and an optional set of product representations. It is used to define an element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">NOTE: The product representations are
        defined as representation maps (at the level of the
        supertype <i>IfcTypeProduct</i>, which gets assigned by
        an element occurrence instance through the
        <i>IfcShapeRepresentation.Item[1]</i> being an
        <i>IfcMappedItem</i>.</font>
> 


A building element type is used to define the common properties of a certain type of a building element that may be applied to many instances of that feature type to assign a specific style. Building element types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The _IfcBuildingElementType_ is an abstract type. Occurrences of subtypes of the _IfcBuildingElementType_ are represented by instances of the appropriate subtypes of _IfcBuildingElement_.

> <small><font color="#0000FF">HISTORY  New entity in
        Release IFC2x Edition 2.</font></small>
>