_IfcConstructionMaterialResource_ identifies a material resource type in a construction project.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _Suppliers_ has been deleted; use _IfcRelAssignsToResource_ to assign an _IfcActor_ to fulfill the role as a supplier. The attribute _UsageRatio_ has been deleted; use _BaseQuantityConsumed_ and _BaseQuantityProduced_ to indicate material usage.

Occurrences of _IfcConstructionMaterialResource_ are consumed (wholly or partially), or occupied during a construction work task (_IfcTask_).

Similar to _IfcConstructionProductResource_, sometimes things such as 5000kg of gravel are already instantiated as an instance of an _IfcProduct_ subtype because it is a result of a work task (for example, &#145;transporting gravel&#146;). In this case, the instance of _IfcConstructionMaterialResource_ can be associated with the product instance &#145;5000kg of gravel&#146; to provide more information for resource uses. Nevertheless, _IfcConstructionMaterialResource_ should only be used to represent resource usage, but not product substances.

> NOTE&nbsp; This entity is not the same as _IfcMaterial_. One one hand, _IfcConstructionMaterialResource_ represents usage of bulk materials such as sand, gravels, nails and so on. Physical manifestations can be instantiated from _IfcProduct_ as well, depending on their uses in the system, and such an _IfcProduct_ object can be assigned to the _IfcConstructionMaterialResource_ object via _IfcRelAssignsToResource_. On the other hand, _IfcMaterial_ is about physical materials that a physical building element consists of, possibly with detailed material layering information."

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcconstructionmaterialresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionmaterialresourcetype.htm">IfcConstructionMaterialResourceType</a></td></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcConstructionMaterialResource Object Typing</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcconstructionmgmtdomain/Qto_ConstructionMaterialResourceBaseQuantities.xml">Qto_ConstructionMaterialResourceBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcConstructionMaterialResource Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Resource Type Assignment

The [Resource Type Assignment](../../templates/resource-type-assignment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcgeographicelement.htm">IfcGeographicElement</a></td><td>Indicates a physical element manifesting the resource such as a pile of sand.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcConstructionMaterialResource Resource Type Assignment</p></td></tr></table>

  
  
{ .use-head}
Resource Cost

The [Resource Cost](../../templates/resource-cost.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>CostType</b></th><th><b>CostName</b></th><th><b>ValueType</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Material</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The amount incurred per unit volume of the material.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcConstructionMaterialResource Resource Cost</p></td></tr></table>

  
  
{ .use-head}
Resource Quantity

The [Resource Quantity](../../templates/resource-quantity.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>QuantityType</b></th><th><b>QuantityName</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcquantityresource/lexical/ifcquantityvolume.htm">IfcQuantityVolume</a></td><td>GrossVolume</td><td>The unit volume of material used, such as cubic meters of concrete.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcConstructionMaterialResource Resource Quantity</p></td></tr></table>