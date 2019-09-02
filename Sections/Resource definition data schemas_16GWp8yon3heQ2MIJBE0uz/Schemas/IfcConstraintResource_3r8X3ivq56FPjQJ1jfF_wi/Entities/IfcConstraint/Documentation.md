An _IfcConstraint_ is used to define a constraint or limiting value or boundary condition that may be applied to an object or to the value of a property.

_IfcConstraint_ may be associated with any subtype of _IfcRoot_ (unless restricted in specific subtypes) through the _IfcRelAssociatesConstraint_ relationship in the _IfcControlExtension_ schema, or may be associated with _IfcProperty_ by _IfcPropertyConstraintRelationship_.

A constraint must have a name applied through the _IfcConstraint.Name_ attribute and optionally, a description through _IfcConstraint.Description_. The grade of the constraint (hard, soft, advisory) must be specified through _IfcConstraint.ConstraintGrade_ or _IfcConstraint.UserDefinedGrade_ whilst the source, creating actor and time at which the constraint is created may be optionally asserted through _IfcConstraint.ConstraintSource_, _IfcConstraint.CreatingActor_ and _IfcConstraint.CreationTime_.

A constraint may also have additional external information (such as classification or document information) associated to it by _IfcExternalReferenceRelationship_, accessible through inverse attribute _IfcConstraint.HasExternalReferences_

> HISTORY&nbsp; New entity in IFC2.0

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; CreationTime changed to IfcDateTime for ISO 8601 representation, HasExternalReferences new inverse attribute.