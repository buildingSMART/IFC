An _IfcResourceConstraintRelationship_ is a relationship entity that enables a constraint to be related to one or more resource level objects.

An _IfcResourceConstraintRelationship_ allows for the specification of a constraint to be applied to many entity types. An important case is to apply constraints to properties. The constraints applied therefore enable a property to carry values identifying requirements as well as those identifying the fulfilment of those requirements.

> EXAMPLE&nbsp; Figure 1 shows how a constraint may be applied to a property within a property set. For simplicity, only the mandatory attributes are shown as asserted. It shows how a property 'ThingWeight' which has a nominal value of 19.5 kg has two constraints that are logically aggregated by an AND connection. One of the constraints has a benchmark of 'GREATERTHANOREQUALTO' whilst the second has a benchmark of 'LESSTHANOREQUALTO'. This means that the constraint must lie between these two bounding values. The relating constraint is instantiated as an objective named as 'Weight Constraint' and qualified as a SPECIFICATION constraint. The two related constraints are both specified as metrics since they can have specific values.

> !["Constraint usage for properties"](../../../figures/IfcResourceConstraintRelationship_fig-1.png "Figure 1 &mdash; Resource constraint relationship")

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Renamed from IfcPropertyConstraintRelationship and extended to apply to all resource level entities. Subtyped from _IfcResourceLevelRelationship_.