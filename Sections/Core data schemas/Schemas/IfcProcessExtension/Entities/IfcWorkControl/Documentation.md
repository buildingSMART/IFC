An _IfcWorkControl_ is an abstract supertype which captures information that is common to both _IfcWorkPlan_ and _IfcWorkSchedule_.

> HISTORY&nbsp; New entity in IFC2x

{ .change-ifc2x4}
> CHANGE IFC4&nbsp; Corrected assignment of resources to work control in documentation. Assignment of tasks to work control updated based on changes of task time definitions and the introduction of a summary task. Identifier has been renamed (now Identification) and promoted to supertype _IfcControl_

A work control may have resources assigned to it. This is handled by the _IfcRelAssignsToControl_ relationship. A work control should also define a context that gives further information about its usage. If no special context information is required then the _IfcProject_ instance as a global context should be used instead. An explicit link between the work control and the _IfcProject_ via _IfcRelDeclares_ should then be provided.

The attribute _IfcWorkControl.Purpose_ is used to define the purpose of either a work schedule or a work plan. In the case of _IfcWorkPlan_, the purpose attribute can be used to determine if the work plan is for cost estimating, task scheduling or some other defined purpose.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcworkcontrol.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcprocessextension/Pset_WorkControlCommon.xml">Pset_WorkControlCommon</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcWorkControl Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Control Assignment

The [Control Assignment](../../templates/control-assignment.htm) concept applies to this entity.

From IFC4 onwards the assignment of tasks to the work control is handled by the _IfcRelAssignsToControl_ relationship. _IfcRelAssignsTasks_ as used in previous IFC releases has been deleted and can not be used any longer. Another change in IFC4 is that it is not necessary to assign each task to a work control as it is regarded to be sufficient if the summary task (root task in the task hierarchy defined through _IfcRelNests_ relationships) is assigned to a work control.