Common definition to capture the basic flow properties of a fluid typically used within a flow distribution system.

In cases where an attribute has a SingleValue specified, the corresponding TimeSeries value shall be omitted. Contrarily, when a TimeSeries value is specified, the corresponding SingleValue shall be omitted.

_IfcFluidFlowProperties_ is a statically defined property set and should be attached to the instance(s) of the _IfcDistributionPort_ through the _IfcRelDefinesByProperties_ relationship. Where two ports are joined together via the _IfcRelConnectsPorts_ relationship, instances of the _IfcFluidFlowProperties_ can be shared.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2x.<br>
    	</font>