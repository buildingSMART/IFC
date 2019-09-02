This objectified relationship, _IfcRelContainedInSpatialStructure_, is used to assign elements to a certain level of the spatial project structure. Any element can only be assigned once to a certain level of the spatial structure. The question, which level is relevant for which type of element, can only be answered within the context of a particular project and might vary within the various regions.

> EXAMPLE&nbsp; A multi-storey space is contained (or belongs to) the building storey at which its ground level is, but it is referenced by all the other building storeys, in which it spans. A lift shaft might be contained by the basement, but referenced by all storeys, through which it spans.

The containment relationship of an element within a spatial structure has to be a hierarchical relationship; an element can only be contained within a single spatial structure element. The reference relationship between an element and the spatial structure need not be hierarchical; that is, an element can reference many spatial structure elements.

> NOTE&nbsp; The reference relationship is expressed by _IfcRelReferencedInSpatialStructure_.

Predefined spatial structure elements to which elements can be assigned are

* site as _IfcSite_ 
* building as _IfcBuilding_ 
* storey as _IfcBuildingStorey_ 
* space as _IfcSpace_ 

Occurrences of the same element type can be assigned to different spatial structure elements depending on the context of the occurrence.

> EXAMPLE&nbsp; A wall might be normally assigned to a storey, however the curtain wall might be assigned to the building and the retaining wall in the terrain might be assigned to the site.

Figure 1 shows the use of _IfcRelContainedInSpatialStructure_ to assign a stair and two walls to two different levels within the spatial structure.

!["fig1"](../../../figures/ifcrelcontainedinspatialstructure-fig1.png "Figure 1 &mdash; Relationship for spatial structure containment")

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x}
> IFC2x CHANGE&nbsp; The data type of the attribute _RelatedElements_ has been changed from _IfcElement_ to its supertype _IfcProduct_ with upward compatibility for file based exchange.