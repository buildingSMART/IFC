An _IfcRelAssignsTasks_ is a relationship class that assigns an _IfcTask_ to an _IfcWorkControl_. The assignment is further qualified by attaching an _IfcScheduleTimeControl_ to the assignment to give the time constraints of the work task, when assigned to a work plan or schedule.

> <font color="#0000FF" size="-1">HISTORY: New class in IFC 2x
		</font>

**Use Definitions**

The inherited attributes have the following meaning:

* _SELF\IfcRelAssigns.RelatedObjects_ - is the reference to the related _IfcTask_, which is assigned to the work control. The task gets the time information from the reference to the _IfcScheduleTimeControl_.
* _SELF\IfcRelAssignsToControl.RelatingControl_ - is the reference to the relating _IfcWorkControl_ (either a work plan or a work schedule) which gets a task assigned.

Each task in a work schedule may have a set of associated time criteria that define information about when the task should be completed. This time information is separated from the the actual work task into the _IfcScheduleTimeControl_ class. Where the work schedule requires that the task and the time control are brought together, this is achieved through the use of the _IfcRelAssignsTask_ class.