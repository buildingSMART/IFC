﻿A spatial structure element is the generalization of all spatial elements that might be used to define a spatial structure. That spatial structure is often used to provide a project structure to organize a building project.

A spatial project structure might define as many levels of decomposition as necessary for the building project. Elements within the spatial project structure are:

* site as _IfcSite_
* facility as _IfcFacility_, or specifically
    * building as IfcBuilding
    * bridge as IfcBridge

* facility part as _IfcFacilityPart_, or specifically
    * storey as IfcBuildingStorey 
    * bridge part as IfcBridgePart

* space as _IfcSpace_

or aggregations or parts thereof. The composition type declares an element to be either an element itself, or an aggregation (complex) or a decomposition (part). The interpretation of these types is given at each subtype of _IfcSpatialStructureElement_.

The _IfcRelAggregates_ is defined as an 1-to-many relationship and used to establish the relationship between exactly two levels within the spatial project structure. Finally the highest level of the spatial structure is assigned to _IfcProject_ using the _IfcRelAggregates_.

The subtypes of _IfcSpatialStructureElement_ relate to other elements and systems by establishing the following relationships:

* **Containment of elements** : _IfcRelContainedInSpatialStructure_ by inverse attribute _ContainsElements_, used to assign any element, like building elements, MEP elements, etc. to the spatial structure element in which they are primarily contained.
* **Reference of elements** : _IfcRelReferencedInSpatialStructure_ by inverse attribute _ReferencesElements_, used to reference any element, like building elements, MEP elements, etc. in spatial structure elements, other then the one, where it is contained.
* **Reference of systems** : _IfcRelServicesBuildings_ by inverse attribute _ServicedBySystems_, used to reference a sytem, like a building service or electrical distribution system, a zonal system, or a structural analysis system, that is assigned to this spatial structure element.

The subtypes of _IfcSpatialStructureElement_ relate to each other by using the _IfcRelAggregates_ relationship to build the project spatial structure. Figure 1 shows the use of _IfcRelAggregates_ to establish a spatial structure including site, building, building section and storey. More information is provided at the level of the subtypes.

!["fig1"](../../../../../../figures/ifcspatialstructureelement-spatialstructure.png "Figure 1 &mdash; Spatial structure element composition")

> HISTORY&nbsp; New entity in IFC2x.

{ .spec-head}
Informal Propositions:

1. The spatial project structure, established by the _IfcRelAggregates_, shall be acyclic.
2. A site should not be (directly or indirectly) associated to a building, storey or space.
3. A building should not be (directly or indirectly) associated to a storey or space.
4. A storey should not be (directly or indirectly) associated to a space.
