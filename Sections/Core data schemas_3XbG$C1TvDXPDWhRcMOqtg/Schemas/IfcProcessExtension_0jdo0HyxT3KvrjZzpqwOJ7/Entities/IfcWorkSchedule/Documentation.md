An _IfcWorkSchedule_ represents a task schedule in a work plan, which in turn can contain a set of schedules for different purposes.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0</font>

**Use Definitions**

An _IfcWorkSchedule_ includes a set of elements (created through relating schedule time controls to tasks) with references to the resources used for the tasks included in the work schedule. Additionally, through the _IfcWorkControl_ abstract supertype, the actors creating the schedule can be specified and schedule time information such as start time, finish time, and total float of the schedule can also be specified.

_IfcWorkSchedule_ can reference a project (i.e. the single _IfcProject_ instance). The documents of the _IfcWorkSchedule_ can be referenced by the _IfcRelAssociatesDocuments_ relationship. Moreover, a work schedule can include other work schedules as sub-items through _IfcRelNests_ relationship.