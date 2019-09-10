The distribution element _IfcDistributionFlowElement_ defines occurrence elements of a distribution system that facilitate the distribution of energy or matter, such as air, water or power.

> <font size="-1">EXAMPLEs of distribution flow elements are 
        ducts, pipes, wires, fittings, equipment, etc.
	  </font>

The _IfcDistributionFlowElement_ utilizes the following capabilities mainly through inverse references to objectified relationships:

* Grouping - being part of a logical group of objects
* Classification - assigned reference to an external classification
* Documentation - assigned reference to an external documentation
* Type - reference to the product type information for the element occurrence
* Properties - reference to all attached properties, including quantities
* Cost control - reference to cost elements associated with this distribution element
* Work processes - reference to work tasks, in which this distribution element participates
* Aggregation - aggregated together with other elements to form an aggregate 
* Connection - connectivity to other elements, including the definition of the connection or joint

The _IfcDistributionFlowElement_ defines the occurrence of a distribution element within the spatial context of a project. The parameters that define the type of the distribution element and/or its shape are defined by the _IfcDistributionFlowElementType_ subtypes, which is related by the inverse relationship IsDefinedBy pointing to _IfcRelDefinesByType_.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionFlowElementCommon](../../psd/IfcSharedBldgServiceElements/Pset_DistributionFlowElementCommon.xml){ target="SOURCE"}: common property set for distribution flow element occurrences 

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

****Containment Use Definition****

The _IfcDistributionFlowElement_, like any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second (optional) relationship is the aggregation within an element assembly.

* The _IfcDistributionFlowElement_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of _IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The _IfcDistributionFlowElement_ may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype. In this case it should not be additionally contained in the project spatial hierarchy, i.e. SELF\IfcElement.ContainedInStructure should be _NIL_.

****Geometry Use Definitions****

The geometric representation of _IfcDistributionFlowElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. If an _IfcRepresentationMap_ is defined for the _IfcFlowElementType_ or one of its subtypes, then the _IfcDistributionFlowELement_ utilizes it through the _IfcMappedItem_. Included geometric representations are:

**Local Placement**

The local placement is defined in the supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_ which can define an absolute placement, relative placement, or grid reference, with each defining the local coordinate system referenced by all geometric representations. If given, the PlacementRelTo relationship of _IfcLocalPlacement_, shall point to the referenced _IfcProduct_. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**Informal propositions for local placement**:

1. If the LocalPlacement is specified, then all aggregated components should use this placement as their relative placement.

**Geometric Representations**

Currently, the use of 'SweptSolid', 'Clipping', 'Brep' and 'MappedRepresentation' representations are supported. In addition, the general representation types 'SurfaceModel' and 'BoundingBox' are allowed. The geometry use definitions for 'BoundingBox', 'SurfaceModel' and 'Brep' are explained at _IfcBuildingElement_. The geometry use definitions for 'SweptSolid' and 'Clipping' are identical to those explained in detail at _IfcBeam_.

**MappedRepresentation**

In addition to the standard and advanced geometric representation of _IfcFlowDistributionElement_ that is defined using the SweptSolid or Clipping geometry, the MappedRepresentation shall be supported as it allows for reusing the geometry definition of the flow distribution element type at all occurrences of the same type. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_: 'Body'
* _RepresentationType_: 'MappedRepresentation'

The same constraints as those given for the standard SweptSolid and the advanced SweptSolid and Clipping geometric representations shall apply to the MappedRepresentation of the _IfcRepresentationMap_.
