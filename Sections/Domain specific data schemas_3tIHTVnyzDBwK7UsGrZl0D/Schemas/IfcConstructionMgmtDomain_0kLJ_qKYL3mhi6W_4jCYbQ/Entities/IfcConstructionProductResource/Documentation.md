_IfcConstructionProductResource_ defines the role of a product that is consumed (wholly or partially), or occupied in the performance of construction.

> HISTORY&nbsp; New entity in IFC2.0. Renamed from IfcProductResource in IFC2x.

Occurrences of _IfcConstructionProductResource_ are usage of products to assist the process of construction. More specifically, they are usage of products that result from some construction processes and that are then used as resources to facilitate further construction. For instance, formworks can be instantiated as products resulting from the process &#145;constructing formwork&#146;. However, they are used as resources in the process &#145;pouring concrete&#146; in a later stage of the project.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcconstructionproductresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionproductresourcetype.htm">IfcConstructionProductResourceType</a></td></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcConstructionProductResource Object Typing</p></td></tr></table>

  
  
{ .use-head}
Resource Assignment

The [Resource Assignment](../../templates/resource-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcelement.htm">IfcElement</a></td><td>Indicates a physical element manifesting the resource such as nails (in bulk).</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcConstructionProductResource Resource Assignment</p></td></tr></table>

  
  
{ .use-head}
Resource Cost

The [Resource Cost](../../templates/resource-cost.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>CostType</b></th><th><b>CostName</b></th><th><b>ValueType</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Product</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The unit cost for purchasing the product.</td></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Shipping</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The unit cost for transporting the product.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcConstructionProductResource Resource Cost</p></td></tr></table>

  
  
{ .use-head}
Resource Quantity

The [Resource Quantity](../../templates/resource-quantity.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>QuantityType</b></th><th><b>QuantityName</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcquantityresource/lexical/ifcquantitycount.htm">IfcQuantityCount</a></td><td>Product</td><td>The unit count of the product used such as 1 for each or 12 for a dozen.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcConstructionProductResource Resource Quantity</p></td></tr></table>