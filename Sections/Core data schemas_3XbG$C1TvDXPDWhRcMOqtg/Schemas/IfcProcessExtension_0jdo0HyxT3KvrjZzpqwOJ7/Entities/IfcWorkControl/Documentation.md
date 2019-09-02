An _IfcWorkControl_ is an abstract supertype which captures information that is common to both _IfcWorkPlan_ and _IfcWorkSchedule_

> <font color="#0000FF" size="-1">HISTORY: New class in IFC
		Release 2x</font>

**Use Definitions**

A work control may have resources assigned to it, this is handled by the _IfcRelAssignsToControl_ relationship. The assignment of tasks to the work control is handled by the _IfcRelAssignsTasks_ relationship.

The inherited attributes have the following meaning:

_IfcControl.Controls_ - references to the _IfcRelAssignsTasks_, that assign instances of _IfcTask_ including time schedule controls.

_IfcObject.HasAssignments_ - references to the _IfcRelAssignsToResources_, that assigns an instance of _IfcResource_ to the _IfcWorkControl_.

The attribute _IfcWorkControl.Purpose_ is used to define the purpose of either a work schedule or a work plan. In the case of _IfcWorkPlan_, the purpose attribute can be used to determine if the work plan is for cost estimating, task scheduling or some other defined purpose.