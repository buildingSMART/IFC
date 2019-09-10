An _IfcLaborResource_ is used in construction with particular skills or crafts required to perform certain types of construction or management related work.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _Skillset_ has been deleted; use LongDescription to describe the skillset.

The purpose of an _IfcLaborResource_ is to identify a skillset that may be required or used. The skillset identified may be (for instance) charge-hand, foreman, labourer, plumbers mate etc. and provides a designation of a particular level of skill. It can be used to identify the generic type of labour resource that is required for a purpose without having to be specific about the actor (person or organization) providing the resource occurrence. It may be particularly useful when creating an overall plan for a process or processes. For instance, within maintenance or work planning there may be a known task that needs to be done which is planned to require a 'chargehand pipe fitter'. There may be several such labour resources available and so the need to identify which will be used is not necessary at the planning stage.

At a later stage, individual actors can be determined for the labour resources. This is achieved through specifying the actor through _IfcActor_. The actor is then identified as the labour resource occurrence through the _IfcRelAssignsToResource.RelatedResource_ attribute. The _IfcLaborResource_ provides the _IfcRelAssignsToResource_._RelatingResource_ attribute.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifclaborresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifclaborresourcetype.htm">IfcLaborResourceType</a></td></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcLaborResource Object Typing</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcconstructionmgmtdomain/Qto_LaborResourceBaseQuantities.xml">Qto_LaborResourceBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcLaborResource Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Resource Assignment

The [Resource Assignment](../../templates/resource-assignment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifckernel/lexical/ifcactor.htm">IfcActor</a></td><td>Indicates specific people manifesting the resource such as laborers.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcLaborResource Resource Assignment</p></td></tr></table>

  
  
{ .use-head}
Resource Cost

The [Resource Cost](../../templates/resource-cost.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>CostType</b></th><th><b>CostName</b></th><th><b>ValueType</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Standard</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>Wages incurred for work during standard hours.</td></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Overtime</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>Wages incurred for work during overtime hours.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcLaborResource Resource Cost</p></td></tr></table>

  
  
{ .use-head}
Resource Quantity

The [Resource Quantity](../../templates/resource-quantity.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>QuantityType</b></th><th><b>QuantityName</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcquantityresource/lexical/ifcquantitytime.htm">IfcQuantityTime</a></td><td>Labor</td><td>Quantity of labor, typically per hour.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcLaborResource Resource Quantity</p></td></tr></table>
