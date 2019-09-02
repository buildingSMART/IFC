The distribution flow element _IfcFlowController_ defines the occurrence of elements of a distribution system that are used to regulate flow through a distribution system (e.g., damper, valve, switch, relay, etc.). Its type is defined by _IfcFlowControllerType_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_FlowControllerDamper](../../psd/IfcSharedBldgServiceElements/Pset_FlowControllerDamper.xml){ target="SOURCE"}: property set for damper flow controller occurrences 
* [Pset_FlowControllerFlowMeter](../../psd/IfcSharedBldgServiceElements/Pset_FlowControllerFlowMeter.xml){ target="SOURCE"}: property set for flowmeter flow controller occurrences 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowController_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.