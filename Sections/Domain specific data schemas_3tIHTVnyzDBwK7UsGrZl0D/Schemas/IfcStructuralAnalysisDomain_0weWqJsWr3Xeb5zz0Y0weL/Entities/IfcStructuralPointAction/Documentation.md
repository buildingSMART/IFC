This entity defines an action which acts on a point. A point action is typically connected with a point connection. It may also be connected with a curve member or curve connection, or surface member or surface connection.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Attributes in the supertypes _IfcStructuralActivity_ and _IfcStructuralAction_ changed. Use definitions changed, informal propositions added.

****Coordinate Systems****:

See definitions at _IfcStructuralActivity_.

****Topology Use Definitions****:

Standard Case:  
If connected with a point item, instances of _IfcStructuralPointAction_ shall not have an _ObjectPlacement_ nor a _Representation_. It is implied that the placement and representation of the action is the same as the structural item.

Special Case 1:  
If connected with a curve item or surface item, instances of _IfcStructuralPointAction_ shall have an _ObjectPlacement_ and _Representation_, containing an _IfcVertexPoint_. See _IfcStructuralActivity_ for further definitions.

> NOTE&nbsp; In order to model concentrated actions on a curve or surface item, _IfcStructuralCurveAction_ or _IfcStructuralSurfaceAction_ of type DISCRETE is preferable since they do not require an extra topology representation in this case. An _IfcStructuralPointAction_ should be used for a concentrated action on a curve or surface item only when an explicit vertex point representation is actually desired.

Special Case 2:  
If not connected with a structural item (which may happen in an incomplete or conceptual model), a point action should have an _ObjectPlacement_ and _Representation_, containing an _IfcVertexPoint_. See _IfcStructuralActivity_ for further definitions.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralpointaction.htm)

{ .use-head}
Structural Activity

The [Structural Activity](../../templates/structural-activity.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>AppliedLoad</b></th><th><b>RelatingElement</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadsingleforce.htm">IfcStructuralLoadSingleForce</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralcurveconnection.htm">IfcStructuralCurveConnection</a></td><td>Point force and moment at a point connection.</td></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadsingleforce.htm">IfcStructuralLoadSingleForce</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralcurvemember.htm">IfcStructuralCurveMember</a></td><td>Point force and moment positioned within a curve member.</td></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadsingleforce.htm">IfcStructuralLoadSingleForce</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralsurfacemember.htm">IfcStructuralSurfaceMember</a></td><td>Point force and moment positioned within a surface member.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralPointAction Structural Activity</p></td></tr></table>