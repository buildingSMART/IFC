_IfcCrewResource_ represents a collection of internal resources used in construction processes.

> HISTORY&nbsp; New entity in IFC2.0.

Identification of people and equipment of a crew is achieved through their specification at the level of the component. Therefore, knowing which persons are within a crew is achieved through identifying the persons assigned to each _IfcLaborResource_ within the _IfcCrewResource_. Similarly, identifying that a screwing machine for pipe fitting forms part of the crew is achieved by relating an appropriate instance of _IfcElementComponent_ to the _IfcConstructionEquipmentResource_ forming an element of the _IfcCrewResource_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcConstructionResource_: [Object Documentation](../../templates/object-documentation.htm), [Object Constraint](../../templates/object-constraint.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Object Nesting](../../templates/object-nesting.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifccrewresource.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifccrewresourcetype.htm">IfcCrewResourceType</a></td></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcCrewResource Object Typing</p></td></tr></table>