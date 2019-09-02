An _IfcCostItem_ can be calculated based on quantities from objects through its relationship to _IfcRelAssignsToControl_.

For quantity-based costing, _IfcElement_, _IfcTask_, or _IfcResource_ occurrence subtypes may be used. Multiple elements may be assigned of the same or different types, using _IfcPhysicalQuantity_ entities defined at each object. Each _IfcPhysicalQuantity_ type must be identical (for example, all values are _IfcAreaQuantity_) such that they can be added together.

For rate-based costing (specifically for _IfcCostScheduleTypeEnum.SCHEDULEOFRATES_), a single _IfcTypeProduct_, _IfcTypeProcess_, or _IfcTypeResource_ subtype may be used to reflect rates for occurrences of such types. This enables the possibility to generate a quantity-based cost schedule for occurrences based on types with rate-based cost schedules.

_IfcRelAssignsToControl_ is also used in the opposite direction to link the root _IfcCostItem_ to an _IfcCostSchedule_ where _RelatingControl_ is the _IfcCostSchedule_.

Figure 1 illustrates cost item assignment derived from building elements. The _IfcRelAssignsToControl_ relationship indicates building elements for which quantities are derived. Not shown, costs may also be derived from building elements by traversing assignment relationships from the assigned _IfcProduct_ to _IfcProcess_ to _IfcResource_, where all costs ultimately originate at resources. It is also possible for cost items to have assignments from processes or resources directly.

!["cost item"](../../../figures/ifccostitem-assignment.png "Figure 1 &mdash; Cost assignment")