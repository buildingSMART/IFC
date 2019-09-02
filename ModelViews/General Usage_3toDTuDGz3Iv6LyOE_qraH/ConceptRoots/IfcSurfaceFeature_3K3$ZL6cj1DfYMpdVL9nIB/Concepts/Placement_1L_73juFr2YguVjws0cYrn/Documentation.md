The local placement for _IfcSurfaceFeatureElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* In case of features which are part of an element type, absolute placement into the type object's implied coordinate system shall be used.
* In case of features which are voiding an element occurrence, the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the respective element.