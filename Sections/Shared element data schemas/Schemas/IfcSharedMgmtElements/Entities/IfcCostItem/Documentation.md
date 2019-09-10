An _IfcCostItem_ describes a cost or financial value together with descriptive information that describes its context in a form that enables it to be used within a cost schedule.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Modified in IFC 2x2.</font>

**Use Definitions**

An _IfcCostItem_ can be used to represent the cost of goods and services, the execution of works by a process, lifecycle cost and much more.

_IfcCostItem_ brings together the value and currency concepts available through the _IfcCostResource_ schema with the identification, naming and descriptive powers that all non-resource entities in the model inherit from _IfcRoot_.

Each instance of _IfcCostItem_ may have a name and a description. Depending on the use for which the cost is intended, these values should be asserted on the basis of agreement. For instance, the name attribute could be used to provide a common value that enables distinct instances to be brought together in a nesting arrangement (see below) whilst the description attribute could be used to provide the typical text that would be used for item description in a costing schedule.

An _IfcCostItem_ can nest other instances of _IfcCostItem_ through its relationships to _IfcRelNests_. This can be used to enable the development of complex groups of costs as may be found in cost schedules through to pages, sections and complete cost schedules.

Instances of _IfcCostItem_ can be assigned to an _IfcCostSchedule_ through the _IfcRelSchedulesCostItems_ relationship class.

Instances of _IfcCostItem_ are used for cost estimates, budgets, etc., where a variety of identification codes are used extensively to identify the meaning of the cost. Examples include project phase codes, CSI codes, takeoff sequence numbers, cost accounts, etc. The IFC model allows for all classes that are ultimately subtypes of _IfcObject_ to inherit the ability to have one or more instances of _IfcClassificationNotation_ to be assigned. Where identification codes are required, the generic IFC classification facility should be used.