The _IfcScheduleTimeControl_ captures the time-related information about a process including the different types (i.e. actual, or scheduled) of starting and ending times, duration, float times, etc.

> <font color="#0000FF" size="-1">HISTORY: Existing class in
		R1.5.1, Renamed to IfcScheduleTimeControl in R2.0.</font>

**Use Definitions**

Scheduled and actual durations of a task and all float times should be derived within an application from relevant start and finish times that are also attributes of this class. Note that they are not directly derived within the IFC specification at this stage due to the differences in data type between time measures date/time selections.

The critical nature of an _IfcScheduleTimeControl_ may also be derived within an application by comparing relevant start and finish date/time selections but is not derived within the IFC specification at this stage.
