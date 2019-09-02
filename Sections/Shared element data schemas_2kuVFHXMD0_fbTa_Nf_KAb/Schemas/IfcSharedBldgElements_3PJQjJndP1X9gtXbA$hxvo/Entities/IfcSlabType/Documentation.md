The element type _IfcSlabType_ defines commonly shared information for occurrences of slabs. The set of shared information may include:

* common properties within shared property sets
* common material information
* common material layer definitions
* common shape representations

> NOTE&nbsp; It is illegal to share shape representations as representation maps for occurrences of _IfcSlabStandardCase_.

It is used to define a slab specification (i.e. the specific product information, that is common to all occurrences of that product type). Slab types may be exchanged without being already assigned to occurrences.

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

The occurrences of the _IfcSlabType_ within building models are represented by instances of _IfcSlabStandardCase_ if the _IfcSlabType_ has a single associated _IfcMaterialLayerSet_; otherwise they are represented by instances of _IfcSlab_, or _IfcSlabElementedCase_.

> HISTORY&nbsp; New entity in IFC2x2.

{ .spec-head}
Informal Propositions:

1. The material assignment, if provided using the _IfcRelAssociatesMaterial_ relationship, shall not reference the _IfcMaterialLayerSetUsage_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcslabtype.htm)

{ .use-head}
Material Layer Set

The [Material Layer Set](../../templates/material-layer-set.htm) concept applies to this entity.

The material of the _IfcSlabType_ is defined by the _IfcMaterialLayerSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcSlabType_, if there is at least one occurrences. of _IfcSlabStandardCase_ for this type.

The shared material layer set definition is defined by assigning an _IfcMaterialLayerSet_ (see material use definition above). The _IfcMaterialLayer_ refers to one or several of _IfcMaterial_ that is the common for all slab occurrence, if used. It is only applicable if the _IfcSlabType_ has only occurrences of type _IfcSlabStandardCase_ (see definition of _IfcSlabStandardCase_ for further information).

> NOTE&nbsp; Since each individual instance of _IfcSlabStandardCase_ defines its own _IfcMaterialLayerSetUsage_ including the offset from the reference plane, the same _IfcSlabType_ can be used independently of the reference plane alignment of its occurrences.

  
  
{ .use-head}
Type Body Geometry

The [Type Body Geometry](../../templates/type-body-geometry.htm) concept applies to this entity.