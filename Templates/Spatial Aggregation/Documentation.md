Provision of a spatial structure of the project by aggregating spatial structure elements. The spatial structure is a hierarchical tree of spatial structure elements (site, building, storey, space) ultimately assigned to the project. Composition refers to the relationship to a higher level element (e.g. this storey is part of a building), decomposition refers to the relationship to lower level elements (e.g. this storey has spaces).

The default requirements stipulated by this **concept template** are:

*  the order of spatial structure elements being included in the concept "Spatial Structure" are from high to low level: _IfcProject, IfcSite, IfcBuilding, IfcBuildingStorey, IfcSpace_.
*  Composition shall only be to an element at the same, or higher level.
*  Decomposition shall only be to an element at the same or lower level.

A **model view definitio**n shall clearly define any further restriction to the applicability of the Composition and Decomposition. if it differs from the default.
