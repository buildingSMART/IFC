A building system is a group by which building elements are grouped according to a common function within the building.

> HISTORY&nbsp; New entity in IFC4.

The group _IfcBuildingSystem_ defines the occurrence of a specialized system for use within the context of a building and finishing fabric. Important functionalities for the description of a building system are derived from supertypes:

* From _IfcSystem_ it inherits the ability to couple the building system via _IfcRelServicesBuildings_ to one or more _IfcSpatialElement_ subtypes as necessary.

* From _IfcGroup_ it inherits the inverse attribute _IsGroupedBy_, pointing to the relationship class _IfcRelAssignsToGroup_. This allows to group building elements (instances of _IfcBuildingElement_ subtypes, _IfcFurnishingElement_ subtype, _IfcElementAssembly_ and _IfcTransportElement_).

* From _IfcObjectDefinition_ it inherits the inverse attribute _IsDecomposedBy_ pointing to the relationship class _IfcRelAggregates_. It provides the hierarchy between the separate (partial) building systems.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcbuildingsystem.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgelements/Pset_BuildingSystemCommon.xml">Pset_BuildingSystemCommon</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLifeFactors.xml">Pset_ServiceLifeFactors</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcBuildingSystem Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcbuildingsystem.htm">IfcBuildingSystem</a></td><td> Building systems may be aggregated into subsystems.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcBuildingSystem Object Aggregation</p></td></tr></table>

  
  
{ .use-head}
Group Assignment

The [Group Assignment](../../templates/group-assignment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingelement.htm">IfcBuildingElement</a></td><td>Building elements participating in the building system.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcBuildingSystem Group Assignment</p></td></tr></table>
