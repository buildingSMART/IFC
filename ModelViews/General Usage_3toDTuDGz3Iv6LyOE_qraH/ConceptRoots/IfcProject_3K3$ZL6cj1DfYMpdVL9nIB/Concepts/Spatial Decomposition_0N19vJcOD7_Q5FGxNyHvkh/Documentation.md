The _IfcProject_ is used to reference the root of the spatial structure of a building or other construction project (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together, and to the _IfcProject_, by using the objectified relationship _IfcRelAggregates_.

The following constraints are applied to using the relationshio _IfcRelAggregates_ in context of _IfcProject_

> NOTE&nbsp; The anomaly to use the composition structure through _IfcRelAggregates_ for assigning the uppermost spatial container to _IfcProject_ is due to upward compatibility reasons with earlier releases of this standard.

* _IfcProject_.Decomposes -- it shall be NIL, i.e. the _IfcProject_ shall be on top of the root of the spatial structure tree.
* _IfcProject_.IsDecomposedBy -- referencing (_IfcSite_ || _IfcBuilding_ || _IfcSpatialZone_) by using _IfcRelAggregates_.RelatedObjects. The _IfcSite_, _IfcBuilding_, or _IfcSpatialZone_ being referenced shall be the root of the spatial structure.

Figure 1 illustrates project relationships with spatial structures, elements, and element type libraries.

!["spatial decomposition relationships"](../../../figures/ifcproject_fig-2.png "Figure 1 &mdash; Project spatial structure, products and product type library")