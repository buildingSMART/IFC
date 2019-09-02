Instances of the entity _IfcStructuralResultGroup_ are used to group results of structural analysis calculations and to capture the connection to the underlying basic load group. The basic functionality for grouping inherited from _IfcGroup_ is used to collect instances from _IfcStructuralReaction_ or its respective subclasses.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; WHERE rule added.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralresultgroup.htm)

{ .use-head}
Group Assignment

The [Group Assignment](../../templates/group-assignment.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralreaction.htm">IfcStructuralReaction</a></td><td>Structural reactions of the result group.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralResultGroup Group Assignment</p></td></tr></table>