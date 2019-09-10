An _IfcAppliedValueRelationship_ is a relationship class that enables applied values of cost or environmental impact to be aggregated together as components of another applied value.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Name changed in IFC 2x2 from
		IfcCostValueRelationship.</font>

**Use Definitions**

Dependency relationships can exist between applied values on the basis that one particular value may be determined by operations on one or more other values. This is captured through the _IfcAppliedValueRelationship_ entity. In this relationship, one instance of _IfcAppliedValue_ acts as the principal (_IfcAppliedValueRelationship.ComponentOf_) whose value may be determined from the instances of _IfcAppliedValue_ that are defined as its components (_IfcAppliedValueRelationship.Components_)

An _IfcAppliedValueRelationship_ has an ArithmeticOperator attribute that specifies the form of arithmetical operation implied by the relationship.

A practical consideration when using the applied value relationship is that when the arithmetic operator is ADD, then the type of the _IfcAppliedValue.AppliedValue_ attribute will be _IfcMeasureWithUnit_ or _IfcMonetaryMeasure_ while if the arithmetic operator is MULTIPLY, then the type of the _IfcAppliedValue.AppliedValue_ attribute for one instance of _IfcAppliedValue_ will be _IfcMeasureWithUnit_ or _IfcMonetaryMeasure_ while for other instances it will be _IfcRatioMeasure_.

**Example**

A relationship exists between applied value A and applied values B, C and D such that the value of A is determined by the addition of B, C and D such that:

A = B + C + D

![Adding Applied Values](images/AppliedValueRelationshipSimple.gif)

It is possible to develop more complex applied value specifications by creating hierarchies of applied value relationships. In the diagram below, the development of a applied value is shown whereby, because B = E \* F and D = G \* H \* J, then:

A = ((E \* F) + C + (G \* H \* J))

![AddMultiply Applied Values](images/AppliedValueRelationshipComplex.gif)
