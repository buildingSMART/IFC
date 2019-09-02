Instances of _IfcStructuralCurveConnection_ describe edge 'nodes', i.e. edges where two or more surface members are joined, or edge supports. Edge curves may be straight or curved.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Attribute _Axis_ added, allowing for skewed supports. Use definitions added.

****Coordinate Systems****:

See definitions at _IfcStructuralItem_. The local coordinate system is established by the reference curve given by topology representation and by the attribute _Axis_. The local x axis is parallel with the tangent on the reference curve. The local z axis is located in the surface which is created by sweeping _Axis_ along the reference curve and is directed according to _Axis_. The local y axis is directed such that x,y,z form a right-handed Cartesian coordinate system.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralcurveconnection.htm)

{ .use-head}
Reference Topology

The [Reference Topology](../../templates/reference-topology.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>RepresentationType</b></th><th><b>Topology</b></th></tr>
<tr><td>Edge</td><td><a href="../../ifctopologyresource/lexical/ifcedge.htm">IfcEdge</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralCurveConnection Reference Topology</p></td></tr></table>