An _IfcCostSchedule_ brings together instances of _IfcCostItem_ either for the purpose of identifying purely cost information as in an estimate for constructions costs, bill of quantities etc. or for including cost information within another presentation form such as an order (of whatever type)

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Modified in IFC 2x2</font>

**Use Definitions**

An _IfcCostSchedule_ is ultimately a subtype of _IfcRoot_ and consequently inherits its identifying, naming and description attributes.

In addition to the global unique identifier, an _IfcCostSchedule_ may be assigned a specific local unique identifier.

The name attribute may be used to give an overall title or name to the _IfcCostSchedule_.

The description attribute may be used to provide further descriptive narrative. This may include specific comments that can be applied.

An _IfcCostSchedule_ may be assigned a status that determines its current level of development or agreement. In the case of an 'APPROVED' status, this should only be set after an approval has been given through the association of an instance of _IfcApproval_.

An _IfcCostSchedule_ may also be declared as being of a particular type. A number of predefined types are included through the _IfcCostScheduleTypeEnum_ enumeration.