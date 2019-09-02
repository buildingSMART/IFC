A system is an organized combination of related parts within an AEC product, composed for a common purpose or function or to provide a service. A system is essentially a functionally related aggregation of products. The grouping relationship to one or several instances of _IfcProduct_ (the system members) is handled by _IfcRelAssignsToGroup_.

> NOTE&nbsp; The use of _IfcSystem_ often applies to the representation of building services related systems, such as the piping system, cold water system, etc. Members within such a system may or may not be connected using the connectivity related entities (through _IfcDistributionPort_).

> HISTORY&nbsp; New entity in IFC1.0

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcGroup_: [Group Assignment](../../templates/group-assignment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcsystem.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLifeFactors.xml">Pset_ServiceLifeFactors</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcSystem Property Sets for Objects</p></td></tr></table>