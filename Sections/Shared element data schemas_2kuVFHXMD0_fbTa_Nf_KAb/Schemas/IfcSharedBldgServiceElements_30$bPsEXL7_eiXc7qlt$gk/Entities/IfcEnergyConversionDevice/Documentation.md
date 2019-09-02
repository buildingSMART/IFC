The distribution flow element _IfcEnergyConversionDevice_ defines the occurrence of a device used to perform energy conversion or heat transfer and typically participates in a flow distribution system. Its type is defined by _IfcEnergyConversionDeviceType_ or its subtypes.

_IfcEnergyConversionDevice_ is a container entity that aggregates all components of the device it represents. The aggregation is handled via the _IfcRelAggregates_ relationship.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_EnergyConversionDeviceCoil](../../psd/IfcSharedBldgServiceElements/Pset_EnergyConversionDeviceCoil.xml){ target="SOURCE"}: property set for coil energy conversion device occurrences 
* [Pset_EnergyConversionDeviceSpaceHeaterPanel](../../psd/IfcSharedBldgServiceElements/Pset_EnergyConversionDeviceSpaceHeaterPanel.xml){ target="SOURCE"}: property set for panel space heater energy conversion device occurrences 
* [Pset_EnergyConversionDeviceSpaceHeaterSectional](../../psd/IfcSharedBldgServiceElements/Pset_EnergyConversionDeviceSpaceHeaterSectional.xml){ target="SOURCE"}: property set for sectional space heater energy conversion device occurrences 

> <font size="-1">
    	NOTE: This entity has been renamed from <i>IfcHeatTransferDevice</i> in 
        IFC R2x.
    	</font>

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcEnergyConversionDevice_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.