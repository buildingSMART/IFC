A spatial zone is a non-hierarchical and potentially overlapping decomposition of the project under some functional consideration. A spatial zone might be used to represent a thermal zone, a construction zone, a lighting zone, a usable area zone. A spatial zone might have its independent placement and shape representation.

> NOTE&nbsp; The _IfcSpatialZone_ is different to the _IfcZone_ entity by allowing an own placement and shape representation, whereas _IfcZone_ is only a grouping of _IfcSpace_'s.

> HISTORY&nbsp; New entity in IFC4.

{ .use-head}
Attribute Use Definition

The _IfcSpatialZone_ inherits and declares these attributes that shall have the following meaning:

* _Name_: A number or designator provided by the user or system for the spatial element, e.g. a space number "1-003", could also be a running number provided by default by the application
* _LongName_: Name of the spatial element provided by the user, e.g. a space name "Office".
* _Description_: Any additional description provided by the user, e.g. a space description "Corner office with habour view".
* _ObjectType_: reserved for typing of spatial elements in case of _PredefinedType_ = .USERDEFINED., restrictions on applicable values might be published in view definitions or implementer agreements.