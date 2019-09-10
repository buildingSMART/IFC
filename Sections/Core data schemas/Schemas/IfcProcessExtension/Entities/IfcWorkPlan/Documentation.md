An _IfcWorkPlan_ represents work plans in a construction or a facilities management project.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0 </font>

**Use Definitions**

A work plan contains a set of work schedules for different purposes (including construction and facilities management). Through inheritance from _IfcWorkControl_, it also have references to all the activities (i.e. _IfcTask_) and resources used in the work schedules.

A work plan has information such as start date, finish date, total free float, and so on. _IfcWorkPlan_ can also refer to the construction project represented by the single _IfcProject_ instance.