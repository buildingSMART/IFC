The element type _IfcWallType_ defines commonly shared information for occurrences of walls. The set of shared information may include:

* common properties within shared property sets
* common material information
* common material layer definitions
* common shape representations

> NOTE&nbsp; It is illegal to share shape representations as representation maps for occurrences of _IfcWallStandardcase_.

It is used to define a wall specification (i.e. the specific product information, that is common to all occurrences of that product type). Wall types may be exchanged without being already assigned to occurrences.

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

Occurrences of the _IfcWallType_ within building models are represented by instances of _IfcWallStandardCase_ if the _IfcWallType_ has a single associated _IfcMaterialLayerSet_; otherwise they are represented by instances of _IfcWall_, or _IfcWallElementedCase_. Occurrences of the _IfcWallType_ within structural analysis models are represented by instances of _IfcStructuralSurfaceMember_, or its applicable subtypes.

> HISTORY&nbsp; New entity in IFC2x2.

{ .spec-head}
Informal Propositions:

1. The material assignment, if provided using the _IfcRelAssociatesMaterial_ relationship, shall not reference the _IfcMaterialLayerSetUsage_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcwalltype.htm)

{ .use-head}
Material Layer Set

The [Material Layer Set](../../templates/material-layer-set.htm) concept applies to this entity.

The material of the _IfcWallType_ is defined by the _IfcMaterialLayerSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcWallType_, if there is at least one occurrences. of _IfcWallStandardCase_ for this type.

The shared material layer set definition is defined by assigning an _IfcMaterialLayerSet_ (see material use definition above). The _IfcMaterialLayer_ refers to one or several of _IfcMaterialLayer_ that is the common for all wall occurrence, if used. It is only applicable if the _IfcWallType_ has only occurrences of type _IfcWallStandardCase_ (see definition of _IfcWallStandardCase_ for further information).

> NOTE&nbsp; Since each individual instance of _IfcWallStandardCase_ defines its own _IfcMaterialLayerSetUsage_ including the offset from the wall axis, the same _IfcWallType_ can be used independently of the axis alignment of its occurrences.

  
  
{ .use-head}
Type Body Geometry

The [Type Body Geometry](../../templates/type-body-geometry.htm) concept applies to this entity.