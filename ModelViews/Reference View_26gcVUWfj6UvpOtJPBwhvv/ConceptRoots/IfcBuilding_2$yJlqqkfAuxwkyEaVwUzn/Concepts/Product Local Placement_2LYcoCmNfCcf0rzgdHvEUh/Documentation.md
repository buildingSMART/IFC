The local placement for _IfcBuilding_ is defined by its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which establishes the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the subtype of _IfcSpatialStructureElement_ that is referenced by the _Spatial Decomposition_ concept (usually of type _IfcSite_).
* If the _IfcBuilding_ is the uppermost spatial structure element, the _PlacementRelTo_ shall not be set.