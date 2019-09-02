**Definition from ISO 6707-1:1989**: Non load bearing wall positioned on the outside of a building and enclosing it.

**Definition of IAI**: Exterior wall of a building which is an assembly of components, hung from the edge of the floor/roof structure rather than bearing on a floor. Curtain wall is represented as a building element assembly and implemented as a subtype of _IfcBuildingElement_ that uses an _IfcRelAggregates_ relationship.

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC Release 2.0
		  </font>
>

****Property Set Use Definition****:

The property sets relating to the _IfcCurtainWall_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcCurtainWall_ are part of this IFC release:

* [Pset_CurtainWallCommon](../../psd/IfcSharedBldgElements/Pset_CurtainWallCommon.xml){ target="SOURCE"}: common property set for all curtain wall occurrences

****Geometry Use Definitions**:**

The geometric representation of _IfcCurtainWall_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Independent geometric representations, as described below, should only be used when the _IfcCurtainWall_ is not defined as an aggregate. If defined as an aggregate, the geometric representation is the sum of the representations of the components within the aggregate.

**Local placement**

The local placement for _IfcCurtainWall_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

If the _IfcCurtainWall_ establishes an aggregate, then all contained elements (defined by the _IsDecomposedBy_ inverse attribute) shall be placed relative to the _IfcCurtainWall.ObjectPlacement_.

**_Geometric Representation_**

Currently, the use of 'BoundingBox', 'SurfaceModel', 'Brep' and 'MappedRepresentation' representations of _IfcCurtainWall_ are supported. The conventions to use these representations are given at the level of the supertype, _IfcBuildingElement_.