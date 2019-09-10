The _IfcSpaceType_ defines a list of commonly shared property set definitions of a space and an optional set of product representations. It is used to define an space specification (i.e. the specific space information, that is common to all occurrences of that space type).

> <small>NOTE  The product representations are defined as
        representation maps (at the level of the supertype
        <i>IfcTypeProduct</i>, which gets assigned by an element
        occurrence instance through the
        <i>IfcShapeRepresentation.Item[1]</i> being an
        <i>IfcMappedItem</i>.</small>
> 


A space type is used to define the common properties of a certain type of space that may be applied to many instances of that type to assign a specific style. Space types may be exchanged without being already assigned to occurrences.

> <small>NOTE  The space types are often used to represent
        space catalogues, less so for sharing a common
        representation map. Space types in a space catalogue
        share same space classification and a common set of space
        requirement properties.</small>
> 


The occurrences of _IfcSpaceType_ are represented by instances of _IfcSpace_.

> <small><font color="#0000FF">HISTORY  New entity in
        Release IFC2x Edition 3.</font></small>
>