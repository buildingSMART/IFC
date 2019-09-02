The material of the _IfcPlateType_ is defined by the _IfcMaterialLayerSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcPlateType_, if there is at least one occurrences of _IfcPlateStandardCase_ for this type.

The shared material layer set definition is defined by assigning an _IfcMaterialLayerSet_ (see material use definition above). The _IfcMaterialLayer_ refers to one or several of _IfcMaterial_ that is the common for all plate occurrence, if used. It is only applicable if the _IfcPlateType_ has only occurrences of type _IfcPlateStandardCase_ (see definition of _IfcPlateStandardCase_ for further information).

> NOTE&nbsp; Since each individual instance of _IfcPlateStandardCase_ defines its own _IfcMaterialLayerSetUsage_ including the offset from the reference plane, the same _IfcPlateType_ can be used independently of the reference plane alignment of its occurrences.