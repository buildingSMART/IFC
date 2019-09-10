_IfcConstructionEquipmentResource_ is usage of construction equipment to assist in the performance of construction. Construction Equipment resources are wholly or partially consumed or occupied in the performance of construction.

> HISTORY&nbsp; New entity in IFC2.0.

Occurrences of _IfcConstructionEquipmentResource_ are products that are used as resources to assist the process of construction. More specifically, they are products that are standalone items brought to a project to fulfil a particular purpose. Examples might be a tower crane or other mobile crane, a screwing machine, or a lifting hoist.

Instances of any subtype of _IfcProduct_ may be assigned to the equipment resource using _IfcRelAssignsToResource_ in order to characterize the equipment further, as described at the supertype _IfcResource_. Examples of relevant subtypes of _IfcProduct_ are _IfcTransportElement_, _IfcDiscreteAccessory_, or _IfcProxy_ (for particular cases where more precise usage details are not available)

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcconstructionequipmentresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionequipmentresourcetype.htm">IfcConstructionEquipmentResourceType</a></td></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcConstructionEquipmentResource Object Typing</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcconstructionmgmtdomain/Qto_ConstructionEquipmentResourceBaseQuantities.xml">Qto_ConstructionEquipmentResourceBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcConstructionEquipmentResource Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Resource Assignment

The [Resource Assignment](../../templates/resource-assignment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifctransportelement.htm">IfcTransportElement</a></td><td>Indicates a physical element manifesting the resource such as a crane.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcConstructionEquipmentResource Resource Assignment</p></td></tr></table>

  
  
{ .use-head}
Resource Cost

The [Resource Cost](../../templates/resource-cost.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>CostType</b></th><th><b>CostName</b></th><th><b>ValueType</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Usage</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The amount incurred for acquiring the equipment, such as rental fees or depreciation.</td></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Operation</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The amount incurred for operating the equipment, such as fuel and maintenance.</td></tr>
<tr><td><a href="../../ifccostresource/lexical/ifccostvalue.htm">IfcCostValue</a></td><td>Deployment</td><td><a href="../../ifcmeasureresource/lexical/ifcmonetarymeasure.htm">IfcMonetaryMeasure</a></td><td>The amount incurred for mobilizing and decomissioning the equipment.</td></tr>
<tr><td>IfcEnvironmentalImpactValue</td><td>RenewableEnergyConsumption</td><td><a href="../../ifcmeasureresource/lexical/ifcenergymeasure.htm">IfcEnergyMeasure</a></td><td>Quantity of renewable energy used as defined in ISO 21930:2007.</td></tr>
<tr><td>IfcEnvironmentalImpactValue</td><td>NonRenewableEnergyConsumption</td><td><a href="../../ifcmeasureresource/lexical/ifcenergymeasure.htm">IfcEnergyMeasure</a></td><td>Quantity of non-renewable energy used as defined in ISO 21930:2007.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcConstructionEquipmentResource Resource Cost</p></td></tr></table>

  
  
{ .use-head}
Resource Quantity

The [Resource Quantity](../../templates/resource-quantity.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>QuantityType</b></th><th><b>QuantityName</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcquantityresource/lexical/ifcquantitytime.htm">IfcQuantityTime</a></td><td>Operation</td><td>The unit basis for operating the equipment, such as an hour.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcConstructionEquipmentResource Resource Quantity</p></td></tr></table>