For the most common case of an _IfcDistributionElement_ subtype containing ports of a particular _PredefinedType_ that all belong to the same distribution system, the _IfcDistributionElement_ is assigned to the _IfcDistributionSystem_ via the _IfcRelAssignsToGroup_ relationship, where _IfcDistributionPort_'s are implied as part of the corresponding system based on their _PredefinedType_. An _IfcDistributionElement_ may belong to multiple systems, however only one _IfcDistributionSystem_ of a particular _PredefinedType_.

For rare cases where an _IfcDistributionElement_ subtype contains ports of the same _PredefinedType_ yet different ports belong to different systems, alternatively each _IfcDistributionPort_ may be directly assigned to a single _IfcDistributionSystem_ via the _IfcRelAssignsToGroup_ relationship, where the _PredefinedType_ must match. Such assignment indicates that the _IfcDistributionSystem_ assigned from the _IfcDistributionPort_ overrides any such system of the same _PredefinedType_ assigned from the containing _IfcDistributionElement_, if any.

Additionally, an _IfcDistributionSystem_ may in turn be assigned to an _IfcDistributionPort_ indicating the host or origination of the system using _IfcRelAssignsToProduct_.

> EXAMPLE&nbsp; A gas-powered hot water heater may have three ports: GAS, DOMESTICCOLDWATER, and DOMESTICHOTWATER. The heater is a member of two systems (GAS and DOMESTICCOLDWATER), and hosts one system (DOMESTICHOTWATER) at the corresponding port.

Figure 1 illustrates a distribution system for an electrical circuit.

!["Instance diagram for electrical circuit"](../../../figures/IfcDistributionSystem-01.png "Figure 1 &mdash; Distribution system assignment")