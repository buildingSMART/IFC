**Definition of IAI**: The railing is a frame assembly adjacent to human circulation spaces and at some space boundaries where it is used in lieu of walls or to complement walls. Designed to aid humans, either as an optional physical support, or to prevent injury by falling. A list of references to accessory/mounting hardware for this railing might be given by including these assessories (_IfcDiscreteAssessory_) through the objectified relationship _IfcRelAggregates_.

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC Release 2.0
		  </font>
>

****Property Set Use Definition****:

The property sets relating to the _IfcRailing_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcRailing_ are part of this IFC release:

* [Pset_RailingCommon](../../psd/IfcSharedBldgElements/Pset_RailingCommon.xml){ target="SOURCE"}: common property set for all railing occurrences

****Geometry Use Definitions****

The geometric representation of _IfcRailing_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local placement**

The local placement for _IfcRailing_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level
* If the _IfcRailing_, however, is used by an _IfcStair_ or _IfcRamp_, and this container class defines its own local placement, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the aggregate.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representation_**

Currently the use of 'BoundingBox', 'SurfaceModel', 'Brep' and 'MappedRepresentation' representations of _IfcRailing_ are supported. The conventions to use these representations are given at the level of the supertype, _IfcBuildingElement_.