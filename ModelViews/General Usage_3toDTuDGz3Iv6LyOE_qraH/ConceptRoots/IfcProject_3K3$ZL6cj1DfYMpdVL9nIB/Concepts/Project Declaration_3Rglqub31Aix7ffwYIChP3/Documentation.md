The _IfcProject_ is also the context for other information about the construction project such as a work plan. Non-product structures are assigned by their first level object to _IfcProject_ using the _IfcRelDeclares_ relationship. The _IfcProject_ provides the context for work plans (or other non-product based) descriptions of the construction project. It is handled by the objectified relationship _IfcRelDeclares_.

> NOTE&nbsp; The spatial structure and the schedule structure can be decomposed. For example the _IfcBuilding_ can be decomposed into _IfcBuildingStorey_'s, and the _IfcWorkPlan_ can be decomposed into _IfcWorkSchedule_'s.

> NOTE&nbsp; The products and tasks can be decomposed further. For example the _IfcCurtainWall_ can be decomposed into _IfcMember_ and _IfcPlate_, the _IfcTask_ can be decomposed into other _IfcTask_'s.

> NOTE&nbsp; The products and tasks can have direct linking relationships. For example the _IfcCurtainWall_ can be assigned to a _IfcTask_ as an input or output for a construction schedule.

Figure 1 illustrates the use of _IfcProject_ as context for work plans or work schedules.

!["project relationships"](../../../figures/ifcproject_fig-1.png "Figure 1 &mdash; Project spatial and work plan structure")