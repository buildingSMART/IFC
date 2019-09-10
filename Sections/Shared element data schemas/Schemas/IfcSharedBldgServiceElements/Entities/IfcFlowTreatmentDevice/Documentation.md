The distribution flow element _IfcFlowTreatmentDevice_ defines the occurrence of a device typically used to remove unwanted matter from a fluid, either liquid or gas, and typically participates in a flow distribution system (e.g., air filter). Its type is defined by _IfcFlowTreatmentDeviceType_ or its subtypes.

_IfcFlowTreatmentDevice_ is a container entity that aggregates all components of the device it represents. The aggregation is handled via the _IfcRelAggregates_ relationship.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 

> <font size="-1">
    	NOTE: This entity has been renamed from <i>IfcTreatmentDevice</i> in 
        IFC R2x.
    	</font>

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2x.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowTreatmentDevice_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.