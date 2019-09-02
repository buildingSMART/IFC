The _IfcProject_ is also the context for other information about the construction project such as a work plan. Non-product structures are assigned by their first level object to _IfcProject_ using the _IfcRelDeclares_ relationship.

The _IfcProject_ provides the context for spatial elements and the associated products, and for work plans (or other non-product based) descriptions of the construction project. It is handled by two distinct relationship objects as shown in Figure 2.

> NOTE&nbsp; The spatial structure and the schedule structure can be decomposed. For example the _IfcBuilding_ can be decomposed into _IfcBuildingStorey_'s, and the _IfcWorkPlan_ can be decomposed into _IfcWorkSchedule_'s.

> NOTE&nbsp; The products and tasks can be decomposed further. For example the _IfcCurtainWall_ can be decomposed into _IfcMember_ and _IfcPlate_, the _IfcTask_ can be decomposed into other _IfcTask_'s.

> NOTE&nbsp; The products and tasks can have direct linking relationships. For example the _IfcCurtainWall_ can be assigned to a _IfcTask_ as an input or output for a construction schedule.

> NOTE&nbsp; The anomaly to use the composition structure through _IfcRelAggregates_ for assigning the uppermost spatial container to _IfcProject_ is due to upward compatibility reasons with earlier releases of this standard.

Figure 1 illustrates the context for project libraries that in return provide a context to the library items assigned to it. Product types are an example for items that can be included in a project library.

!["project relationships"](../../../figures/IfcProject_fig-1.png "Figure 1 &mdash; Project spatial and work plan structure")

Figure 2 illustrates project relationships with spatial structures, products, and type libraries.

!["project relationships"](../../../figures/IfcProject_fig-2.png "Figure 2 &mdash; Project spatial structure, products and product type library")