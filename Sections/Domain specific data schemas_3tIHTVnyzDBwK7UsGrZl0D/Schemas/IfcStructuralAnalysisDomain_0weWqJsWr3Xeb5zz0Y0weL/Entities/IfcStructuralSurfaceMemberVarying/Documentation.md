This entity describes surface members with varying section properties. The properties are provided by means of _Pset_StructuralSurfaceMemberVaryingThickness_ via _IfcRelDefinesByProperties_, or by means of aggregation: An instance of _IfcStructuralSurfaceMemberVarying_ may be composed of two or more instances of _IfcStructuralSurfaceMember_ with differing section properties. These subordinate members relate to the instance of _IfcStructuralSurfaceMemberVarying_ by _IfcRelAggregates_.

> NOTE&nbsp; It is recommended that structural activities (actions or reactions) are not connected with aggregated _IfcStructuralSurfaceMemberVarying_ but only with the _IfcStructuralSurfaceMember_s in the aggregation. That way, difficulties in interpretation of local coordinates are avoided.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Use definition changed and attributes deleted.

****Coordinate Systems****:

See definitions at _IfcStructuralItem_ and _IfcStructuralSurfaceMember_. The local coordinates of an aggregate are generally undefined since continuity of local coordinates of the parts is not ensured.

****Material Use Definition****

In case of aggregation, only the individual parts (direct instances of _IfcStructuralSurfaceMember_) carry material and thickness information. Otherwise, definitions at _IfcStructuralSurfaceMember_ apply.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcStructuralSurfaceMember_: [Material Layer Set Usage](../../templates/material-layer-set-usage.htm), [Reference Topology](../../templates/reference-topology.htm), [Structural Connectivity](../../templates/structural-connectivity.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralsurfacemembervarying.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralanalysisdomain/Pset_StructuralSurfaceMemberVaryingThickness.xml">Pset_StructuralSurfaceMemberVaryingThickness</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralSurfaceMemberVarying Property Sets for Objects</p></td></tr></table>