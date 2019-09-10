Instances of _IfcStructuralCurveMember_ describe edge members, i.e. structural analysis idealizations of beams, columns, rods etc.. Curve members may be straight or curved.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Attribute _Axis_ and WHERE rule added. Use definitions changed.

****Coordinate Systems****:

See definitions at _IfcStructuralItem_. The local coordinate system is established by the reference curve given by topology representation and by the attribute _Axis_. The local x axis is parallel with the tangent on the reference curve. The local z axis is located in the surface which is created by sweeping _Axis_ along the reference curve and is directed according to _Axis_. The local y axis is directed such that x,y,z form a right-handed Cartesian coordinate system.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralcurvemember.htm)

{ .use-head}
Structural Connectivity

The [Structural Connectivity](../../templates/structural-connectivity.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>StructuralConnection</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralpointconnection.htm">IfcStructuralPointConnection</a></td><td>Point connections at each end of the member.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralCurveMember Structural Connectivity</p></td></tr></table>

  
  
{ .use-head}
Material Profile Set Usage

The [Material Profile Set Usage](../../templates/material-profile-set-usage.htm) concept applies to this entity.

The material of direct instances _IfcStructuralCurveMember_ (in contrast to instances of the subtype _IfcStructuralCurveMemberVarying_) is defined by _IfcMaterialProfileSetUsage_ and attached by the _IfcRelAssociatesMaterial.RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Composite profile beams can be represented by refering to several _IfcMaterialProfile_s within the _IfcMaterialProfileSet_ that is referenced from the _IfcMaterialProfileSetUsage_. In case of tapered members, the material profile usage subtype _IfcMaterialProfileSetUsageDual_ is used which specifies _IfcMaterialProfileSet_s separately at the start and the end of the tapered member.

The material (_IfcMaterial_) in each _IfcMaterialProfile_(_Set_) is specified minimally by a name which corresponds with an agreed upon standardized structural material designation. An external reference to the source which specifies the material designation should be provided. Alternatively, structural material properties may be provided by means of _IfcMechanicalMaterialProperties_ and _IfcExtendedMaterialProperties_.

The profile (_IfcProfileDef_) in each _IfcMaterialProfile_(_Set_) is specified minimally by a name which corresponds with an agreed upon standardized structural profile designation. An external reference to the source which specifies the profile designation should be provided. Alternatively or additionally, explicit profile geometry should be provided by using respective subtypes of _IfcProfileDef_. Alternatively or additionally, structural profile properties may be provided by means of subtypes of _IfcProfileProperties_.

An _IfcProfileDef_ is a two-dimensional geometric object with a x~p~,y~p~ coordinate system. The profile is inserted into the curve member model thus that the origin of x~p~,y~p~ is located at the member's reference curve and that x~p~,y~p~ are parallel with and directed like the local y,z.

> NOTE&nbsp; Due to convention in structural mechanics, axis names of _IfcStructuralCurveMember_ differ from axis names of building elements like _IfcBeamStandardCase_: The extrusion axis of _IfcStructuralCurveMember_ is called x while the extrusion axis of _IfcBeamStandardCase_ is called z. Hence x,y,z of _IfcStructuralCurveMember_ correspond with z,x,y of _IfcBeamStandardCase_.

If the profile is meant to be inserted centrically in terms of structural section properties, it is necessary that the origin of x~p~,y~p~ is identical with the geometric centroid of the profile (commonly also called centre of gravity). If subtypes of _IfcParameterizedProfileDef_ are used which are only singly symmetric or are asymmetric, an explicit translation by _IfcParameterizedProfileDef.Position.Location_ is required then.

If the profile is inserted at its geometric centroid, _IfcMaterialProfileSetUsage.CardinalPoint_ shall be set to 10.

Otherwise, the profile is inserted eccentrically and a different cardinal point should be set accordingly.

> NOTE&nbsp; Another eccentricity model is available independently of eccentric profile specification: The reference curve of the member may be located eccentrically relative to the reference points of the connected _IfcStructuralPointConnection_s. The connection relationship is then established by _IfcRelConnectsWithEccentricity_. Whether one or the other or both eccentricity models may be used is subject to information requirements and local agreements.

  
  
{ .use-head}
Reference Topology

The [Reference Topology](../../templates/reference-topology.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>RepresentationType</b></th><th><b>Topology</b></th></tr>
<tr><td>Edge</td><td><a href="../../ifctopologyresource/lexical/ifcedge.htm">IfcEdge</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcStructuralCurveMember Reference Topology</p></td></tr></table>

Direct instances of _IfcStructuralCurveMember_ shall have a topology representation which consists of one instance of _IfcEdge_ or a subtype, representing the reference curve of the curve member. See definitions at _IfcStructuralItem_ for further specifications.

{ .spec-head}
Informal Propositions:

1. The reference curve must not be parallel with _Axis_ at any point within the curve member's domain.

The local coordinate system is established by the reference curve given by topology representation and by the attribute _Axis_. The local x axis is parallel with the tangent on the reference curve. The local z axis is located in the surface which is created by sweeping _Axis_ along the reference curve and is directed according to _Axis_. The local y axis is directed such that x,y,z form a right-handed Cartesian coordinate system.
