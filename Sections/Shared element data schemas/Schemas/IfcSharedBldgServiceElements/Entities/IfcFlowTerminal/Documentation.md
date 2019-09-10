The distribution flow element _IfcFlowTerminal_ defines the occurrence of a permanently attached element that acts as a terminus or beginning of a distribution system (e.g., air outlet, drain, water closet, sink, etc.). A terminal is typically a point at which a system interfaces with an external environment. Its type is defined by _IfcFlowTerminalType_ or its subtypes.

An _IfcFlowController_ can be either aggregated into the definition of the _IfcFlowTerminal_ using the _IfcRelAggregates_ relationship, or referenced using the _IfcRelConnectsPorts_ objectified relationship.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_FlowTerminalAirTerminal](../../psd/IfcSharedBldgServiceElements/Pset_FlowTerminalAirTerminal.xml){ target="SOURCE"}: property set for air terminal occurrences 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowTerminal_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_FlowTerminalAirTerminal](../../psd/IfcSharedBldgServiceElements/Pset_FlowTerminalAirTerminal.xml){ target="SOURCE"}: Occurrence-specific property set for individual air terminal occurrences. 

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.
