_IfcConstructionResource_ is an abstract generalization of the different resources used in construction projects, mainly labour, material, equipment and product resources, plus subcontracted resources and aggregations such as a crew resource.

A resource represents "use of something" and does not necessarily correspond to a single item such as a person or vehicle, but represents a pool of items having limited availability such as general labor or an equipment fleet. A resource can represent either a generic resource pool (not having any task assignment) or a task-specific resource allocation (having an _IfcTask_ assignment).

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Modified in to promote _ResourceIdentifer_ and _ResourceGroup_ (renamed to _LongDescription_) to supertype _IfcResource_ and add attributes as described.

{ .use-head}
Declaration use definition

A root-level resource (specifically _IfcCrewResource_ or _IfcSubContractResource_) is declared within the project by _IfcRelDeclares_ where _RelatingContext_ refers to the single _IfcProject_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_, and other root-level objects within the project.

{ .use-head}
Assignment use definition

A resource may be assigned to an actor by _IfcRelAssignsToActor_ where _RelatingActor_ refers to an _IfcActor_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_ or other objects. Such relationship indicates the actor responsible for allocating the resource such as partitioning into task-specific allocations, delegating to other actors, and/or scheduling over time. Note that this assignment does not indicate the person or organization performing the work; that is indicated by _IfcRelAssignsToResource_. The actor responsible for the resource may or may not be the same as any actor(s) performing work.

A resource may be assigned to a control by _IfcRelAssignsToControl_ where _RelatingProduct_ refers to an _IfcControl_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_ or other objects. Most commonly an _IfcWorkCalendar_ is assigned indicating availability of the resource, where such calendar is nested within a base calendar or an _IfcWorkPlan_ which in turn is assigned to the _IfcProject_.

A resource may be assigned to a group by _IfcRelAssignsToGroup_ where _RelatingGroup_ refers to an _IfcGroup_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_ or other objects. Most commonly an _IfcAsset_ is assigned indicating the asset to be tracked, where such asset is nested within an _IfcInventory_ which in turn is assigned to the _IfcProject_.

A resource may be assigned to a product by _IfcRelAssignsToProduct_ where _RelatingProduct_ refers to an _IfcProduct_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_ or other objects. Most commonly an _IfcElement_ subtype is assigned indicating the product to be constructed, where such product is connected to a spatial structure which in turn is aggregated within the _IfcProject_.

A resource may be assigned to a process by _IfcRelAssignsToProcess_ where _RelatingProcess_ refers to an _IfcProcess_ and _RelatedObjects_ refers to one or more _IfcConstructionResource_ or other objects. Most commonly an _IfcTask_ is assigned indicating the task to be performed by the resource, where such task is nested within a summary task which in turn is assigned to the _IfcProject_.

A resource may have assignments of other objects using _IfcRelAssignsToResource_ where _RelatingResource_ refers to the _IfcConstructionResource_ and _RelatedObjects_ refers to one or more objects such as _IfcActor_ or _IfcProduct_ subtypes. This relationship indicates specific objects assigned to fulfill resource usage.

Figure 1 illustrates resource assignment.

!["Assignment Use Definition"](../../../figures/IfcConstructionResource-Assignment.png "Figure 1 &mdash; Construction resource assignment use")

{ .use-head}
Baseline use definition

A resource may have any number of baselines defined using the relationship _IfcRelDefinesByObject_ where _RelatingObject_ is the "current" resource and _RelatedObjects_ consists of multiple "baseline" resources, each representing a copy of the resource as it existed at an earlier point in time as shown in Figure 185. Each baseline _IfcConstructionResource_ is identified by its nested _IfcRelAssignsToControl_ relationship to an _IfcWorkSchedule_ having _PredefinedType=BASELINE_, _IfcWorkSchedule.CreationDate_ indicating the date of the baseline, and _IfcWorkSchedule.Name_ indicating the name of the baseline.

!["Baseline Use Definition"](../../../figures/IfcConstructionResource-Baseline.png "Figure 2 &mdash; Construction resource baseline use")

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcconstructionresource.htm)

{ .use-head}
Object Documentation

The [Object Documentation](../../templates/object-documentation.htm) concept applies to this entity.

Documents may be published for work plans consisting of schedules, calendars, tasks, and resources. The relationship _IfcRelAssociatesDocument_ may be used to preserve mappings to such document where _RelatingDocument_ points to an _IfcDocumentReference_ and _RelatedObjects_ includes the _IfcConstructionResource_ as shown in Figure 184. _IfcDocumentReference.ItemReference_ identifies the resource within the scope of the document, such as an integer or guid. The _IfcDocumentReference.ReferencedDocument_ corresponds to the document which is uniquely identified by _IfcDocumentInformation.DocumentId_ and/or _IfcDocumentInformation.PublicationLocation_. Such document mapping allows items in the document to be updated from the building information model and vice-versa.

!["Document Use Definition"](../../../figures/IfcConstructionResource-Document.png "Figure 3 &mdash; Construction resource document use")

  
  
{ .use-head}
Object Constraint

The [Object Constraint](../../templates/object-constraint.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>DataValue</b></th><th><b>Attribute1</b></th><th><b>Attribute2</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcmeasureresource/lexical/ifcpositiveratiomeasure.htm">IfcPositiveRatioMeasure</a></td><td>Usage</td><td>ScheduleUsage</td><td>Indicate fixed usage (such as simultaneous workers) such that changes to ScheduleWork should impact the assigned IfcTask.TaskTime.ScheduleDuration and vice-versa.</td></tr>
<tr><td><a href="../../ifcdatetimeresource/lexical/ifcduration.htm">IfcDuration</a></td><td>Usage</td><td>ScheduleWork</td><td>Indicate fixed work (such as total person-hours) such that changes to ScheduleUsage should impact the assigned IfcTask.TaskTime.ScheduleDuration and vice-versa.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcConstructionResource Object Constraint</p></td></tr></table>

Constraints may be applied to a resource to indicate fixed work (such as total person-hours) or fixed usage (such as simultaneous workers).

  
  
{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresourcetype.htm">IfcConstructionResourceType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcConstructionResource Object Typing</p></td></tr></table>

The resource type may provide shared productivity and cost information, allowing tasks and resources to be selected according to lowest cost and/or shortest duration. Given an _IfcProduct_ of a particular _IfcTypeProduct_ type, an _IfcTypeProcess_ may be selected from those assigned to the product type using _IfcRelAssignsToProduct_, and an _IfcTypeResource_ may be selected from those assigned to the process type using _IfcRelAssignsToProcess_. Then _IfcTask_ and _IfcConstructionResource_ occurrences may be instantiated from the type definitions, applying productivitity and rate information to assigned quantities to calculate _ResourceTime.ScheduleWork_. Task durations can then be calculated by dividing _ResourceTime.ScheduleWork_ by _ResourceTime.ScheduleUsage_.

!["Type Use Definition"](../../../figures/IfcConstructionResource-Type.png "Figure 4 &mdash; Construction resource type use")

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcconstructionmgmtdomain/Pset_ConstructionResource.xml">Pset_ConstructionResource</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcConstructionResource Property Sets for Objects</p></td></tr></table>

For time series properties as shown in Figure 180, each _IfcTimeSeriesValue_ indicates a LIST of values, where the sequence of the value corresponds to the _IfcCostValue_ at _IfcConstructionResource.CostRatesConsumed_. For example, if _CostRatesConsumed_ has two _IfcCostValue_ items in the LIST, "Standard" and "Overtime", then _IfcTimeSeriesValue(IfcDuration('T8H0M0S'),IfcDuration('T2H0M0S'))_ would indicate 8 hours at Standard rate and 2 hours at Overtime rate. If the list of values at _IfcTimeSeriesValue.ListValues_ is less than the size of _CostRatesConsumed_, then subsequent values are considered to be zero.

!["Time Series Use Definition"](../../../figures/IfcConstructionResource-TimeSeries.png "Figure 5 &mdash; Construction resource time series use")

  
  
{ .use-head}
Object Nesting

The [Object Nesting](../../templates/object-nesting.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcconstructionmgmtdomain/lexical/ifcconstructionresource.htm">IfcConstructionResource</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcConstructionResource Object Nesting</p></td></tr></table>

Resources may be decomposed into allocation pools using the _IfcRelNests_ relationship as shown in Figure 181. For example, an _IfcLaborResource_ for "Electrician" may be decomposed into three task-specific _IfcLaborResource_ objects: "Electrical Rough-in", "First Floor Circuits", and "Second Floor Circuits". Both relating and related sides may represent the same _ResourceTime.ScheduleUsage_ quantity (for example, 6 workers time-shared), or the related side may break out _ResourceTime.ScheduleUsage_ quantities for reserved use (for example, 4 workers and 2 workers).

A common scenario is two nesting levels where the first-level resources have no task assignments; while second-level resources have specific task assignments indicating that the resource is subdivided into allocations for specific tasks. While the model allows unlimited nesting of resources, implementer agreements may restrict to two nesting levels with task assignments specifically at the second level.

!["Composition Use Definition"](../../../figures/IfcConstructionResource-Composition.png "Figure 6 &mdash; Construction resource composition use")