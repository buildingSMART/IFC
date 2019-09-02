A structural curve action defines an action which is distributed over a curve. A curve action may be connected with a curve member or curve connection, or surface member or surface connection.

> HISTORY&nbsp; New entity in IFC4.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Former entity _IfcStructuralLinearActionVarying_ from IFC2x2 has been removed and are replaced by this entity.

****Coordinate Systems****:

See definitions at _IfcStructuralActivity_.

****Topology Use Definitions****:

Standard Case:  
If connected with a curve item, instances of _IfcStructuralCurveAction_ shall not have an _ObjectPlacement_ nor a _Representation_. It is implied that the placement and representation of the _IfcStructuralActivity_ is the same as the ones of the member or connection.

Special Case 1:  
If connected with a surface item, instances of _IfcStructuralCurveAction_ shall have an _ObjectPlacement_ and _Representation_, containing an _IfcEdgeCurve_. See _IfcStructuralActivity_ for further definitions.

Special Case 2:  
If not connected with a structural item (which may happen in an incomplete or conceptual model), a curve action should have an _ObjectPlacement_ and _Representation_, containing an _IfcEdgeCurve_. See _IfcStructuralActivity_ for further definitions.

{ .spec-head}
Informal Propositions:

1. If the curve action is of the predefined type CONST, SINUS, or PARABOLA, _SELF\IfcStructuralActivity.AppliedLoad_ must not be of type _IfcStructuralLoadConfiguration_. In case of SINUS and PARABOLA, the load item defines the maximum of the load at the centre of the load distribution.
2. If the curve action is of the predefined type LINEAR, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain two items.
3. If the curve action is of the predefined type POLYGONAL, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain three or more items.
4. If the curve action is of the predefined type DISCRETE, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain two or more items.
5. In case of types LINEAR, POLYGONAL, and DISCRETE, the load items shall have one-dimensional _IfcStructuralLoadConfiguration.Locations_, defining the location of the load samples in local coordinates of the curve action. The load items shall be provided in ascending order according to their locations. The first and the last load item define the extent of the load distribution. 
6. Point actions must be of type DISCRETE, thus contain two or more load points. (Single point loads are modeled by _IfcStructuralPointAction_.)
7. All items in _SELF\IfcStructuralActivity.AppliedLoad\IfcStructuralLoadConfiguration.Values_ shall be of the same entity type.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralcurveaction.htm)

{ .use-head}
Structural Activity

The [Structural Activity](../../templates/structural-activity.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>AppliedLoad</b></th><th><b>RelatingElement</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadlinearforce.htm">IfcStructuralLoadLinearForce</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralcurvemember.htm">IfcStructuralCurveMember</a></td><td>Linear force and moment along a curve member.</td></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadlinearforce.htm">IfcStructuralLoadLinearForce</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralsurfacemember.htm">IfcStructuralSurfaceMember</a></td><td>Linear force and moment positioned within a surface member.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralCurveAction Structural Activity</p></td></tr></table>