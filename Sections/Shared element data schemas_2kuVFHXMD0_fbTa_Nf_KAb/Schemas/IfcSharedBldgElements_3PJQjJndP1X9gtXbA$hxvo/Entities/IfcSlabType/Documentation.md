The element type (_IfcSlabType_) defines a list of commonly shared property set definitions of a slab and an optional set of product representations. It is used to define a slab specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">NOTE: The product representations
are defined as representation maps (at the level of the supertype <i>IfcTypeProduct</i>,
which gets assigned by an element occurrence instance through the <i>IfcShapeRepresentation.Item[1]</i>
being an <i>IfcMappedItem</i>.</font>
>

An _IfcSlabType_&nbsp;is used to define the common properties of a specific slab that may be applied to many instances of that type to assign a specific style. A slab type can be used for a floor slab, a roof slab, a stair landing or a ramp flight. Building element types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The _IfcSlabType_ can have common material (using the inverse relationship _HasAssociations_) or property set information (using _HasPropertySets_) assigned. If present, it does apply equally to all occurrences of the _IfcSlabType_. Property set information may be overridden at the occurrence.

The occurrences of the _IfcSlabType_ are represented by instances of _IfcSlab.&nbsp;_~~or
_IfcRampFlight_~~

> <font color="#0000ff" size="-1">HISTORY:
New entity in Release IFC2x Edition 2.</font>
>

**Informal proposition**:

1. The material assignment, if provided using the _IfcRelAssociatesMaterial_ relationship, shall not reference the _IfcMaterialLayerSetUsage_.