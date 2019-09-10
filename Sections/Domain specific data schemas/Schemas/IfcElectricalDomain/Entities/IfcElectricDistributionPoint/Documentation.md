An _IfcElectricDistributionPoint_ is a flow controller in which instances of electrical devices are brought together at a single place for a particular purpose

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Property Set Use Definition****:

The property sets relating to the _IfcElectricDistributionPoint_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcElectricDistributionPoint_are part of this IFC release:

* [Pset_ElectricDistributionPointCommon](../../psd/IfcElectricalDomain/Pset_ElectricDistributionPointCommon.xml): common property set for all types of an electric distribution point panel, distribution board etc.), if available 

****Use Definitions****

An _IfcElectricDistributionPoint_ provides a housing for an aggregation of different types of instances of electrical distribution elements so that they can be viewed, operated or acted upon from a single place. Each item in the aggregation may have its own geometric representation and location by virtue of being a subtype of _IfcProduct_.

_IfcElectricDistributionPoint_ acts as the relating object in an _IfcRelAggregates_ relationship, the electrical devices that are brought together being the related objects.

****Geometry Use Definitions****

The geometric representation of an occurrence of an _IfcElectricDistributionPoint_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The local placement is defined in the supertype _IfcProduct_. It is defined by a subtype of _IfcObjectPlacement_ which can define an absolute placement, relative placement, or grid reference, with each defining the local coordinate system referenced by all geometric representations. The PlacementRelTo relationship of _IfcLocalPlacement_, if given, shall point to the same _IfcSpatialStructureElement_ which is used in the ContainedInStructure inverse attribute, or to a referenced spatial structure element at a higher level. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**Informal propositions for local placement**:

1. If the LocalPlacement is specified, then all aggregated components should use this placement as their relative placement. 

**Standard Geometric Representation**

Currently, the use of profiles to define the geometry for an occurrence of this class is not supported. The standard geometric representation is defined using explicit geometry.

**B-Rep Representation**

The faceted B-Rep capabilities (with or without voids) shall be supported for B-Rep representation.
