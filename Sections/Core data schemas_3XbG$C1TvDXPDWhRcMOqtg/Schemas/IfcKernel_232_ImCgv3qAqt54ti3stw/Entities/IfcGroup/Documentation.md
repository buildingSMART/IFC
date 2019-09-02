The _IfcGroup_ is an generalization of any arbitrary group. A group is a logical collection of objects. It does not have its own position, nor can it hold its own shape representation. Therefore a group is an aggregation under some non-geometrical / topological grouping aspects.

> <small>NOTE&nbsp; Use <i>IfcRelDecomposes</i>
together with the appropriate subtypes of <i>IfcProduct</i>
to define an aggregation of products that may have its own position and
shape representation.<br>
EXAMPLE&nbsp; An example for a group
is the system, since it groups elements under the aspect of their role,
regardless of their position in a building.</small>

A group can hold any collection of objects (being&nbsp;products, processes, controls, resources, actors or other groups). Thus groups can be nested. An object can be part of zero, one, or many groups. Grouping relationships are not required to be hierarchical.

> <small>NOTE&nbsp; Use <i>IfcRelDecomposes</i>
together with the appropriate subtypes of <i>IfcProduct</i>
to define an hierarchical aggregation of products.</small>

The group collection is handled by an instance of _IfcRelAssignsToGroup_, which assigns all group members to the _IfcGroup_.

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 1.0.</font></small>
>