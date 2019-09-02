_IfcProcess_ is defined as one individual activity or event, that is ordered in time, that has sequence relationships with other processes, which transforms input in output, and may connect to other other processes through input output relationships. An _IfcProcess_ can be an activity (or task), or an event. It takes usually place in building construction with the intent of designing, costing, acquiring, constructing, or maintaining products or other and similar tasks or procedures.

{ .extDef}
> NOTE&nbsp; Definition according to ISO9000:  
> A process is a set of activities that are interrelated or that interact with one another. Processes use resources to transform inputs into outputs. Processes are interconnected because the output from one process becomes the input for another process. In effect, processes are "glued" together by means of such input output relationships.

!["icon diagram"](../../../figures/IfcProcess_icon_fig.png "Figure 1 &mdash; Process relationships and the ICON process diagram.")

> HISTORY&nbsp; New entity in IFC1.0.

{ .change-ifc2x}
> IFC2x CHANGE&nbsp; The attribute _Productivity_ has been removed.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _Identification_ has been promoted from subtypes _IfcTask_ and others.

{ .use-head}
Relationship use definition

Process information relates to other objects by establishing the following relationships:

* **Nesting of processes** : _IfcRelNests_ - A process can contain sub processes and thereby be nested.
* **Sequencing of processes** : _IfcRelSequence_ - Processes can be placed in sequence (including overlapping for parallel tasks), and have predecessors and successors.
* **Assigning process to schedules** : _IfcRelAssignsToControl_ - Activities such as tasks, and predominately summary tasks, are assigned to a work schedule.
* **Having a product assigned to the process as input** : _IfcRelAssignsToProcess_ - Products can be assigned as input to a process, such as for construction process planning.
* **Having a product assigned to the process as output** : _IfcRelAssignsToProduct_ - Products can be assigned as output to a process, such as for construction process planning.
* **Having a control assigned to the process as process control** : _IfcRelAssignsToProcess_ - Items that act as a control onto the process can be assigned to a process, such as for cost management (a cost item assigned to a work task).
* **Having a resource assigned to the process as consumed by the process** : _IfcRelAssignsToProcess_ - Items that act as a mechanism to a process, such as labor, material and equipment in cost calculations.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcprocess.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Risk.xml">Pset_Risk</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcProcess Property Sets for Objects</p></td></tr></table>