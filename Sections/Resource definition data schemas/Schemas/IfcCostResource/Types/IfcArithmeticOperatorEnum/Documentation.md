The _IfcArithmeticOperatorEnum_ specifies the form of arithmetical operation implied by the relationship.

**Enumeration**

* ADD
* DIVIDE
* MULTIPLY
* SUBTRACT

> <font size="-1" color="#0000FF">HISTORY: New enumeration in IFC
		2x2.</font>

**Use Definitions**

There can be only one arithmetic operator for each applied value relationship. This is to enforce arithmetic consistency. Given this consistency, the cardinality of the IfcAppliedValueRelationship.Components attribute is a set of one to many applied values that are components of an applied value.
