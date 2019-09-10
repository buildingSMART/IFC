The _IfcCoveringType_ defines a list of commonly shared property set definitions of an element and an optional set of product representations. It is used to define an element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <small>NOTE The product representations are defined as
        representation maps at the level of the supertype
        <i>IfcTypeProduct</i>, which gets assigned by an element
        occurrence instance through the
        <i>IfcShapeRepresentation.Item[1]</i> being an
        <i>IfcMappedItem</i>.</small>
> 


A covering type is used to define the common properties of a certain type of a covering that may be applied to many instances of that type to assign a specific style. Covering types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCoveringType_ are represented by instances of _IfcCovering_ (or its subtypes).

> <small><font color="#0000FF">HISTORY New entity in
        Release IFC2x Edition 2.</font></small>
> 


**Informal proposition**

1. The material assignment, if provided using the _IfcRelAssociatesMaterial_ relationship, shall not reference the _IfcMaterialLayerSetUsage_.