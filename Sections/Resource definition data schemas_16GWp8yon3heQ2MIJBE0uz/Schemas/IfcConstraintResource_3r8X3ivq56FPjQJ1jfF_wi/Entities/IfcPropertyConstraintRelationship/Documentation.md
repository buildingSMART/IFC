An _IfcPropertyConstraintRelationship_ is a relationship class that enables a constraint to be related to one or more properties.

> <font color="#0000FF" size="-1">HISTORY: New entity in Release IFC2x Edition 2.</font>
>

### Use Definition
An _IfcPropertyConstraintRelationship_ allows for the specification of a constraint to be applied to many properties. The constraints applied therefore enable a property to carry values identifying requirements as well as those identifying the fulfilment of those requirements.

The example below shows how a constraint may be applied to a property within a property set. For simplicity, only the mandatory attributes are shown as asserted. It shows how a property 'ThingWeight' which has a nominal value of 19.5 kg has two constraints that are logically aggregated by an AND connection. One of the constraints has a benchmark of 'GREATERTHANOREQUALTO' whilst the second has a benchmark of 'LESSTHANOREQUALTO'. This means that the constraint must lie between these two bounding values. The relating constraint is instantiated as an objective named as 'Weight Constraint' and qualified as a SPECIFICATION constraint. The two related constraints are both specified as metrics since they can have specific values.

![ConstraintUsage](figures/ConstraintUsageExample.gif)