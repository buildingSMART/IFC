The material of the _IfcWallType_ is defined by the _IfcMaterialLayerSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcWallType_, if there is at least one occurrences. of _IfcWallStandardCase_ for this type.

The shared material layer set definition is defined by assigning an _IfcMaterialLayerSet_ (see material use definition above). The _IfcMaterialLayer_ refers to one or several of _IfcMaterialLayer_ that is the common for all wall occurrence, if used. It is only applicable if the _IfcWallType_ has only occurrences of type _IfcWallStandardCase_ (see definition of _IfcWallStandardCase_ for further information).

> NOTE&nbsp; Since each individual instance of _IfcWallStandardCase_ defines its own _IfcMaterialLayerSetUsage_ including the offset from the wall axis, the same _IfcWallType_ can be used independently of the axis alignment of its occurrences.