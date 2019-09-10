The _IfcConstraintResource_ schema provides for the specification of constraints that can be applied to objects or to properties so as limit or bound their values.

The concept is that a constraint (_IfcConstraint_)may be applied to any object that is ultimately a subtype of _IfcObject_ (through the provision of the relationship class _IfcRelAssociatesConstraint_) or that is an _IfcProperty_ (through the provision of the relationship class _IfcPropertyConstraintRelationship_).

A grade must be also be set for the constraint that establishes whether it is a hard constraint (must be satisfied), a soft constraint (should be satisfied) or simply advisory.

A constraint must be named and may optionally have one or more sources within which it is defined or from which it is taken.

Additionally, a constraint may optionally be assigned a creating actor, creation date and a description.

### Constraint Aggregation
Constraints may be aggregated together via the IfcConstraintAggregationRelationship. This allows complex constraints to be developed based on their logical relationship.

### Constraint Types
Constraint may be either qualitative (an objective constraint) or quantitative (a measured constraint or metric). A qualifier can be applied to an objective constraint that determines the purpose for which it is applied. It may be applied to define the constraining values beyond which building codes may be violated or to limit the selectable range of values as in a specification (e.g. value of A must be greater than A but less than B). Several possible purposes are provided through an enumeration.

A set of benchmark values can be specified for the objective constraint and a set of result values captured for performance comparison purposes.

A measured constraint or metric defines the actual value or values of a constraint. Values can be defined in terms of a benchmark requirement which sets the intent of the constraint i.e. whether the benchmark is greater than (&gt;), less than (&lt;) etc.

The value of a constraint may be defined according to a number of datatypes that are available through a select mechanism.

For instance, a constraint advised by a manufacturer beyond which maintenance must be undertaken on a pump might be qualified as a 'TriggerCondition', named 'PumpMaintenanceCondition', have as its source 'ManufacturerData' and be graded as 'Advisory'. It could have as a single value 10\^-2 / sec as the frequency of vibration and have a benchmark of 'GreaterThanOrEqualTo'.

> <font size="-1" color="#0000FF">HISTORY: New schema in IFC 2x
		containing <i>IfcConstraint</i> and its subtypes, previously in
		<i>IfcControlExtension</i>. Modified in IFC 2x2</font>
