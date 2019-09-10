The distribution flow element _IfcFlowMovingDevice_ defines the occurrence of an apparatus used to distribute, circulate or perform conveyance of fluids, including liquids and gases, and typically participates in a flow distribution system (e.g., pump, fan). Its type is defined by _IfcFlowMovingDeviceType_ or its subtypes.

_IfcFlowMovingDevice_ is a container entity that aggregates all components of the device it represents. The aggregation is handled via the _IfcRelAggregates_ relationship.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_FlowMovingDeviceCompressor](../../psd/IfcSharedBldgServiceElements/Pset_FlowMovingDeviceCompressor.xml){ target="SOURCE"}: property set for compressor occurrences 
* [Pset_FlowMovingDeviceFan](../../psd/IfcSharedBldgServiceElements/Pset_FlowMovingDeviceFan.xml){ target="SOURCE"}: property set for fan occurrences 
* [Pset_FlowMovingDeviceFanCentrifugal](../../psd/IfcSharedBldgServiceElements/Pset_FlowMovingDeviceFanCentrifugal.xml){ target="SOURCE"}: property set for centrifugal fan occurrences 
* [Pset_FlowMovingDevicePump](../../psd/IfcSharedBldgServiceElements/Pset_FlowMovingDevicePump.xml){ target="SOURCE"}: property set for pump occurrences 

> <font size="-1">
    	NOTE: This entity has been renamed <i>IfcFlowMovingDevice</i> in 
        IFC R2x.
    	</font>

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2x.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowMovingDevice_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.