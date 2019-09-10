_IfcPerformanceHistory_ is used to document the actual performance of an occurrence instance over time. It includes machine-measured data from building automation systems and human-specified data such as task and resource usage. The data may represent actual conditions, predictions, or simulations.

The realtime data tracked by performance history takes the form of property sets where all properties are based on time series. Unlike design-based data at occurrences and types, performance-driven data is time-sensitive and may change in realtime by some measurement device. Data may be captured at irregular intervals such as when values change beyond established thresholds, or at regular intervals of specified duration.

#### Declaration use definition
_IfcPerformanceHistory_ may be declared within a project using _IfcRelDeclares_ where _RelatingContext_ refers to the _IfcProject_ and _RelatedDefinitions_ includes the _IfcPerformanceHistory_. Default units (used for property sets) are indicated by the declaring project. Only top-level objects are declared; nested performance history objects (through _IfcRelNests_) do not participate in such relationship.

> HISTORY&nbsp; New entity in IFC2x2.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcperformancehistory.htm)

{ .use-head}
Property Sets for Performance

The [Property Sets for Performance](../../templates/property-sets-for-performance.htm) concept applies to this entity.

The property sets relating to this entity are defined by _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. They are accessible by the _IsDefinedBy_ inverse attribute. Applicable property sets are defined at assigned entities (primarily _IfcDistributionElement_ subtypes) where _IfcPropertySetTemplate.PropertySetType_ is _PSET_PERFORMANCEDRIVEN_.

In addition to standard property sets defined within this specification, if the underlying information source provides metadata (specific type information), then custom property sets may capture such data, where corresponding _IfcPropertySetTemplate_ and _IfcPropertyTemplate_ objects may be defined for such information to be accessed by other applications.

  
  
{ .use-head}
Object Classification

The [Object Classification](../../templates/object-classification.htm) concept applies to this entity.

_IfcPerformanceHistory_ may be classified using _IfcRelAssociatesClassification_ where _RelatingClassification_ refers to an _IfcClassificationReference_ indicating a classification notation. Such classification notation may be used to identify the information such as an address within a building automation system, a work breakdown structure code for tasks, or a cost code for resource allocation.

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifccontrolextension/lexical/ifcperformancehistory.htm">IfcPerformanceHistory</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcPerformanceHistory Object Aggregation</p></td></tr></table>

_IfcPerformanceHistory_ may be decomposed into components using _IfcRelNests_ where _RelatingObject_ refers to the enclosing _IfcPerformanceHistory_ and _RelatedObjects_ contains one or more _IfcPerformanceHistory_ components. Composition indicates breakdown of further detail and may correspond to the hierarchy of objects it represents.

  
  
{ .use-head}
Control Assignment

The [Control Assignment](../../templates/control-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifckernel/lexical/ifcgroup.htm">IfcGroup</a></td><td>A system or zone for which time-based system information is provided, such as overall status parameters of a building control system.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcproduct.htm">IfcProduct</a></td><td>A building space, physical device, or port for which time-based information is provided, such as a chiller or an analog input within a device.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcprocess.htm">IfcProcess</a></td><td>A process for which time-based information is provided, such as an alarm event being raised and acknowledged, or regular and overtime costs incurred for a task.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcresource.htm">IfcResource</a></td><td>A resource for which usage is recorded or planned over time, such as wage rates and number of workers at particular times.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcPerformanceHistory Control Assignment</p></td></tr></table>