_IfcSubContractResource_ is a construction resource needed in a construction process that represents a sub-contractor.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _SubContractor_ has been deleted; use _IfcRelAssignsToResource_ to assign an _IfcActor_ to fulfill the role as the subcontractor. The attribute _JobDescription_ has been deleted; use _LongDescription_ to describe the job.

An _IfcSubContractResource_ can be used in cost estimating and work planning with or without specifying the subcontractor and contract agreement.

The purpose of an _IfcSubContractResource_ is to indicate work of a particular type that is that is to be engaged through the use of a sub-contract. Its aim is to identify the description of the sub-contract work required. It can be used to identify the generic type of sub-contract resource that is required for a purpose without having to be specific about the actor (person or organization) providing the resource occurrence. It may be particularly useful when creating an overall plan for a process or processes. For instance, within maintenance or work planning there may be a known task that needs to be done which is planned to require an 'insulation specialist'.

A subcontract resource may be described at various stages and levels of detail through its assignments:

* Subcontract resource designated for particular tasks
* Actors identified to request bids
* Cost schedules (bids) received from actors
* Project order (work order, change order, etc.) executed

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcsubcontractresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcSubContractResource Object Typing</p></td></tr></table>

  
  
{ .use-head}
Resource Assignment

The [Resource Assignment](../../templates/resource-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifckernel/lexical/ifcactor.htm">IfcActor</a></td><td>Indicates a specific organization to be considered to fulfill the resource or invited to bid on the resource.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcSubContractResource Resource Assignment</p></td></tr></table>