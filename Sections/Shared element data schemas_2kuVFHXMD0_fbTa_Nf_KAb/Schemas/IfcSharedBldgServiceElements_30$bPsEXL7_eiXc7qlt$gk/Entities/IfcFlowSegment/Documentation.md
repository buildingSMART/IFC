The distribution flow element _IfcFlowSegment_ defines the occurrence of a segment of a flow distribution system that is typically straight, contiguous and has two ports (e.g., a section of pipe or duct).

The _IfcFlowSegment_ defines a particular occurrence of a segment inserted in the spatial context of a project. The parameters defining the type of the segment and/or its shape are defined by the _IfcFlowSegmentType_, which is related by the inverse relationship IsDefinedBy pointing to _IfcRelDefinesByType_.

The following parameters shall be given:

* Segment length, taken from the Length attribute in the property set, provides the depth of the extrusion.
* Segment profile dimensions are defined by the NominalDiameterOrWidth and NominalHeight attributes in the property set.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 
* [Pset_FlowSegmentDuctSegment](../../psd/IfcSharedBldgServiceElements/Pset_FlowSegmentDuctSegment.xml){ target="SOURCE"}: property set for duct segment occurrences 
* [Pset_FlowSegmentPipeSegment](../../psd/IfcSharedBldgServiceElements/Pset_FlowSegmentPipeSegment.xml){ target="SOURCE"}: property set for pipe segment occurrences 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcFlowSegment_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The use of local placement is defined at the supertype _IfcDistributionFlowElement_.

**Standard Geometric Representation**

The use of Standard Geometric Representations is defined at the supertype _IfcDistributionFlowElement_.