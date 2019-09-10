_IfcGroup_ is an generalization of any arbitrary group. A group is a logical collection of objects. It does not have its own position, nor can it hold its own shape representation. Therefore a group is an aggregation under some non-geometrical / topological grouping aspects.

> NOTE&nbsp; Use _IfcRelDecomposes_ together with the appropriate subtypes of _IfcProduct_ to define an aggregation of products that may have its own position and shape representation.

> EXAMPLE&nbsp; An example for a group is a system, since it groups elements under the aspect of their role, regardless of their position in a building.

A group can hold any collection of objects (being products, processes, controls, resources, actors or other groups). Thus groups can be nested. An object can be part of zero, one, or many groups. Grouping relationships are not required to be hierarchical nor do they imply a dependency.

> NOTE&nbsp; Use _IfcRelDecomposes_ together with the appropriate subtypes of _IfcProduct_ to define an hierarchical aggregation of products.

A group can be exchanged without having already objects within the group collection.

> HISTORY&nbsp; New entity in IFC1.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The inverse _IsGroupedBy_ relationship is set to 0..n

{ .use-head}
Relationship use definition

Groups are assigned to other objects (such as a process or a resource) by the relationship object that refers to the corresponding object:

* Process: assigned using _IfcRelAssignsToProcess_
* Resource: assigned using _IfcRelAssignsToResource_

Groups can be subjected to a control. The control information is then assigned:

* Controls: affecting the group using _IfcRelAssignsToControl_

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcgroup.htm)

{ .use-head}
Group Assignment

The [Group Assignment](../../templates/group-assignment.htm) concept applies to this entity.
