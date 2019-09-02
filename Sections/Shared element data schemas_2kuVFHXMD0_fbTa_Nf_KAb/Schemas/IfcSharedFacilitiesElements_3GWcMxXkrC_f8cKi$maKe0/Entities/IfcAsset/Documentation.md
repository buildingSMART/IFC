An _IfcAsset_ is a uniquely identifiable grouping of elements acting as a single entity that has a financial value

> <font color="#0000ff" size="-1">HISTORY
New class in IFC 2x. Modified in IFC 2x2</font>

****Use Definitions****

An asset is generally the level of granularity at which maintenance operations are undertaken. An asset is a group that can contain one or more elements. While the value of a component or element can be defined, value is also defined for accounting purposes at the level of the asset.

There are a number of actors that can be associated with an asset, each actor having a role. Principal actors are identified as attributes of the class. Additional actors can be specified through the relationship class _IfcRelAssignsToActor_ in which case roles should be defined through the _IfcActorRole_ class which must be asserted for each defined role.

There are a number of costs that can be associated with an asset, each cost having a role. Principal costs are identified as attributes of the class. Additional costs can be specified through the relationship class _IfcRelAssociatesCost_ in which case roles must be asserted.

Service life data (expected life etc.) can be assigned for one or more assets as _IfcServiceLife_ through the relationship class _IfcRelAssignsToControl_.

The operating function of an asset within an organization may be particularly valuable in situations where one organization provides and maintains core services and another organization adds and maintains terminal services. It can classify who owns and is responsible for the asset. Operating function can be designated through the use of one or more classification notations which will be handled through the relationship class _IfcRelAssociatesClassification_.

****Property Set Use Definition****:

The property sets relating to an _IfcAsset_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcAsset_ are part of this IFC release:

* [Pset_Asset](../../psd/IfcSharedFacilitiesElements/Pset_Asset.xml): specific property set for the properties of an asset, if available 
* [Pset_Reliability](../../psd/IfcSharedFacilitiesElements/Pset_Reliability.xml): specific property set for the properties defining risk that may be associated with an asset or any occurrence of a subtype of _IfcProduct_, if available 
* [Pset_Risk](../../psd/IfcSharedFacilitiesElements/Pset_Risk.xml): specific property set for the properties defining risk that may be associated with an asset or any occurrence of a subtype of _IfcObject_, if available 
* [Pset_Warranty](../../psd/IfcSharedFacilitiesElements/Pset_Warranty.xml): specific property set for the properties relating to a warranty or guarantee that may be associated with an asset, any occurrence of _IfcProduct_ or any occurrence of _IfcSystem_, if available 

****Geometry Use Definitions****

The geometric representation of an _IfcAsset_ is determined by the geometric representations of the products that comprise the asset (since an asset is a subtype of _IfcGroup_)