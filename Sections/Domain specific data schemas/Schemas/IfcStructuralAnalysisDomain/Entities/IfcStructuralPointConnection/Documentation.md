Instances of _IfcStructuralPointConnection_ describe structural nodes or point supports.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Attribute _ConditionCoordinateSystem_ added, allowing for skewed supports. Use definitions added.

****Coordinate Systems****:

See definitions at _IfcStructuralItem_. The local coordinate system is established by the reference point given by topology representation and by the attribute _ConditionCoordinateSystem_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralpointconnection.htm)

{ .use-head}
Reference Topology

The [Reference Topology](../../templates/reference-topology.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>RepresentationType</b></th><th><b>Topology</b></th></tr>
<tr><td>Vertex</td><td><a href="../../ifctopologyresource/lexical/ifcvertexpoint.htm">IfcVertexPoint</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralPointConnection Reference Topology</p></td></tr></table>

Instances of _IfcStructuralPointConnection_ shall have a topology representation which consists of one _IfcVertexPoint_, representing the reference point of the point connection. See definitions at _IfcStructuralItem_ for further specifications.