This entity defines a reaction which occurs distributed over a curve. A curve reaction may be connected with a curve member or curve connection, or surface member or surface connection.

> HISTORY&nbsp; New entity in IFC4.

****Coordinate Systems****:

See definitions at _IfcStructuralActivity_.

****Topology Use Definitions****:

Standard Case:  
If connected with a curve item, instances of _IfcStructuralCurveRection_ shall not have an _ObjectPlacement_ nor a _Representation_. It is implied that the placement and representation of the _IfcStructuralActivity_ is the same as the ones of the member or connection.

Special Case:  
If connected with a surface item, instances of _IfcStructuralCurveReaction_ shall have an _ObjectPlacement_ and _Representation_, containing an _IfcEdgeCurve_. See _IfcStructuralActivity_ for further definitions.

{ .spec-head}
Informal Propositions:

1. If the curve reaction is of the predefined type CONST, _SELF\IfcStructuralActivity.AppliedLoad_ must not be of type _IfcStructuralLoadConfiguration_.
2. If the curve reaction is of the predefined type LINEAR, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain two items.
3. If the curve reaction is of the predefined type POLYGONAL, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain three or more items.
4. If the curve action is of the predefined type DISCRETE, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain two or more items.
5. In case of types LINEAR, POLYGONAL, and DISCRETE, the load items shall have one-dimensional _IfcStructuralLoadConfiguration.Locations_, defining the location of the result samples in local coordinates of the curve reaction. The load items shall be provided in ascending order according to their locations. The first and the last load item define the extent of the result distribution. 
6. If the curve reaction is of the predefined type EQUIDISTANT, _SELF\IfcStructuralActivity.AppliedLoad_ shall be of type _IfcStructuralLoadConfiguration_ and shall contain two or more items. _IfcStructuralLoadConfiguration.Locations_ shall be omitted as it is implicit. The load items shall be provided in ascending order. The first and the last load item are located at the beginning and end of the result distribution, respectively.
7. All items in _SELF\IfcStructuralActivity.AppliedLoad\IfcStructuralLoadConfiguration.Values_ shall be of the same entity type.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralcurvereaction.htm)

{ .use-head}
Structural Activity

The [Structural Activity](../../templates/structural-activity.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>AppliedLoad</b></th><th><b>RelatingElement</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralloadresource/lexical/ifcstructuralloadconfiguration.htm">IfcStructuralLoadConfiguration</a></td><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralcurvemember.htm">IfcStructuralCurveMember</a></td><td>Resulting shear and moment along a curve member.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralCurveReaction Structural Activity</p></td></tr></table>
