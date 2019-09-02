The local placement for _IfcSpace_ is defined at its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the _IfcSpatialStructureElement_ of type _IfcBuildingStorey_ or _IfcSite_ if relative placement is used.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system.