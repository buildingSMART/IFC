The _IfcDistributionChamberElement_ defines a place at which distribution systems and their constituent elements may be inspected or through which they may travel.

An _IfcDistributionChamberElement_ is a formed volume used in a distribution system, such as a sump, trench or manhole. Instances of _IfcSystem_ or _IfcDistributionFlowElement_ may be related to the _IfcDistributionChamberElement_ enabling their location in or at the chamber to be determined.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC 2x2.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcDistributionChamberElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.