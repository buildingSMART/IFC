The distribution flow element _IfcFlowStorageDevice_ defines the occurrence of a device that participates in a distribution system and is used for temporary storage of a fluid such as a liquid or a gas (e.g., tank). Its type is defined by _IfcFlowStorageDeviceType_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_FlowStorageDeviceTank](../../psd/IfcSharedBldgServiceElements/Pset_FlowStorageDeviceTank.xml){ target="SOURCE"}: property set for tank storage device occurrences 

> <font size="-1">
    	NOTE: This entity has been renamed from <i>IfcStorageDevice</i> in 
        IFC R2x.
    	</font>

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2x.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowStorageDevice_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.