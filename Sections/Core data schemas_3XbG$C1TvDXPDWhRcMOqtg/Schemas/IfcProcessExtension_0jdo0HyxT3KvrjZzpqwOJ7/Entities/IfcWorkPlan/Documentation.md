An _IfcWorkPlan_ represents work plans in a construction or a facilities management project.

> HISTORY&nbsp; New entity in IFC2.0

A work plan contains a set of work schedules for different purposes (including construction and facilities management). Contained work schedules are defined through the _IfcRelAggregates_ relationship. Through inheritance from _IfcWorkControl_ it is also possible to define references to activities (for example, _IfcTask_) and resources used in the work plan.

A work plan has information such as start date, finish date, total free float, and so on. _IfcWorkPlan_ can also refer to the construction project represented by the single _IfcProject_ instance (please also check the definition of _IfcWorkControl_).

Figure 1 shows the backbone structure of a work plan that defines (1) contained work schedules through _IfcRelAggregates_ and (2), if not assigned otherwise to contained work schedules, assigned tasks and resources through _IfcRelAssignsToControl_.

If an assigned _IfcTask_ is a root-level task, such task must be declared on the _IfcProject_ using the _IfcRelDeclares_ relationship.

!["work plan instantiation diagram"](../../../figures/ifcworkplan_instantiation_diagram.png "Figure 1 &mdash; Work plan relationships")