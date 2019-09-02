**IfcDistributionPort** may be connected to other objects as follows using the indicated relationship:

* **IfcDistributionPort** (_IfcRelConnectsPorts_) : Indicates a connection to another port having the same type and opposite flow direction. For port connections between elements, the _RelatingPort_ is set to a port having _FlowDirection=SOURCE_ and the _RelatedPort_ is set to a port having _FlowDirection=SINK_. For aggregation scenarios, ports on a device may be mapped to aggregated devices within, in which case ports on the outer device indicate a single _FlowDirection_ but have an additional connection internally to a port on an aggregated inner device. Refer to [IfcUnitaryEquipment](../../ifchvacdomain/lexical/ifcunitaryequipment.htm) for an example.
* _IfcDistributionElement_ (_IfcRelConnectsPortToElement_): For dynamic ports, indicates the containing element. 

Figure 1 illustrates distribution port connectivity.

!["Connection Use Definition"](../../../figures/IfcDistributionPort-Connection.png "Figure 1 &mdash; Distribution port connectivity")