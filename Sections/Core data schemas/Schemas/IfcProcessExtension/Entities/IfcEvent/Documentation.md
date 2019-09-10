An _IfcEvent_ is something that happens that triggers an action or response.

> HISTORY&nbsp; New entity in IFC4

{ .use-head}
Use definitions

_IfcEvent_ is used to capture information about particular things that happen or that may happen. Particularly used in work plans (or process maps) they identify e.g. a point at which a message containing information may be issued or at which a rule or constraint is invoked.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcevent.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifceventtype.htm">IfcEventType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcEvent Object Typing</p></td></tr></table>

The _IfcEvent_ defines the anticipated or actual occurrence of any event; common information about event types is handled by _IfcEventType_.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Risk.xml">Pset_Risk</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcEvent Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Object Nesting

The [Object Nesting](../../templates/object-nesting.htm) concept applies to this entity.

_IfcEvent_ may be contained within an _IfcTask_ using the _IfcRelNests_ relationship. The event is considered active during the time period of the enclosing task (including any assigned _IfcWorkCalendar_); that is such event may be triggered within the task time period but not outside of it. As an _IfcEvent_ is considered to be atomic, no use is anticipated for nesting processes inside the event.

  
  
{ .use-head}
Sequential Connectivity

The [Sequential Connectivity](../../templates/sequential-connectivity.htm) concept applies to this entity.

The relationship _IfcRelSequence_ is used to indicate control flow. An _IfcEvent_ as a predecessor (_IfcRelSequence.RelatingProcess_) indicates that the succeeding process (typically _IfcProcedure_ or _IfcTask_) is triggered in response to the event. An _IfcEvent_ as a successor (_IfcRelSequence.RelatedProcess_) indicates that the completion of the preceeding process causes the event to be triggered. As events have zero duration, the _IfcRelSequence.SequenceType_ attribute has no effect on an _IfcEvent_ but still applies to the opposite end of the relationship if _IfcTask_ is used.

  
  
{ .use-head}
Control Assignment

The [Control Assignment](../../templates/control-assignment.htm) concept applies to this entity.

An _IfcEvent_ may be assigned to an _IfcWorkCalendar_ to indicate times when such event is active using _IfcRelAssignsToControl_; otherwise the effective calendar is determined by the nearest _IfcProcess_ ancestor with a calendar assigned.

  
  
{ .use-head}
Product Assignment

The [Product Assignment](../../templates/product-assignment.htm) concept applies to this entity.

For building operation scenarios, _IfcEvent_ may be assigned to a product (_IfcElement_ subtype) using _IfcRelAssignsToProduct_ to indicate a specific product occurrence that sources the event.

> EXAMPLE&nbsp; An _IfcSensor_ for a motion sensor may have a "Motion Sensed" event. If the _IfcEvent_ is defined by an _IfcEventType_ and the _IfcEventType_ is assigned to a product type (using _IfcRelAssignsToProduct_), then the _IfcEvent_ must be assigned to one or more occurrences of the specified product type using _IfcRelAssignsToProduct_.