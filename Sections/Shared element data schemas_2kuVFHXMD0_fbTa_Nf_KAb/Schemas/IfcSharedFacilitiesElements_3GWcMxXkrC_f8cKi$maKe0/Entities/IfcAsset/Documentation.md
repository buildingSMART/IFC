An asset is a uniquely identifiable grouping of elements acting as a single entity that has a financial value or that can be operated on as a single unit.

An asset is generally the level of granularity at which maintenance operations are undertaken. An asset is a group that can contain one or more elements. Whilst the financial value of a component or element can be defined, financial value is also defined for accounting purposes at the level of the asset.  
  
There are a number of actors that can be associated with an asset, each actor having a role. Actors within the scope of the project are indicated using the [IfcRelAssignsToActor](../../ifckernel/lexical/ifcrelassignstoactor.htm) relationship in which case roles should be defined through the [IfcActorRole](../../ifcactorresource/lexical/ifcactorrole.htm) class; otherwise principal actors are identified as attributes of the class. In the existence of both, direct attributes take precedence.  
  
There are a number of costs that can be associated with an asset, each cost having a role. These are specified through the _OriginalValue_, _CurrentValue_, _TotalReplacementCost_ and _DepreciatedValue_ attributes.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; All attributes made optional and date values changed to use _IfcDate_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcasset.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Asset.xml">Pset_Asset</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcAsset Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Object Classification

The [Object Classification](../../templates/object-classification.htm) concept applies to this entity.

The operating function of an asset within an organization may be particularly valuable in situations where one organization provides and maintains core services and another organization adds and maintains terminal services. It can classify who owns and is responsible for the asset. Operating function can be designated through the use of one or more classification references.

  
  
{ .use-head}
Group Assignment

The [Group Assignment](../../templates/group-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcelement.htm">IfcElement</a></td><td>Physical elements that comprise the asset.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcAsset Group Assignment</p></td></tr></table>