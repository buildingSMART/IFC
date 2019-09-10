Instances of _IfcStructuralSurfaceMember_ describe face members, that is, structural analysis idealizations of slabs, walls, and shells. Surface members may be planar or curved.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Use definitions changed, WHERE rule added.

****Coordinate Systems****:

See definitions at _IfcStructuralItem_. The local coordinate system is established by the reference surface given by topology representation.

****Material Use Definition****

The material of direct instances _IfcStructuralSurfaceMember_ (in contrast to instances of the subtype _IfcStructuralSurfaceMemberVarying_) is defined by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial.RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

The material is specified minimally by a name which corresponds with an agreed upon standardized structural material designation. An external reference to the source which specifies the material designation should be provided. Alternatively, structural material properties may be provided by means of _IfcMechanicalMaterialProperties_ and _IfcExtendedMaterialProperties_.

Direct instances of _IfcStructuralSurfaceMember_ are assumed to be located centrically relative to their reference surface. Their depth is provided in the attribute _Thickness_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstructuralsurfacemember.htm)

{ .use-head}
Material Layer Set Usage

The [Material Layer Set Usage](../../templates/material-layer-set-usage.htm) concept applies to this entity.

The material of direct instances _IfcStructuralSurfaceMember_ (in contrast to instances of the subtype _IfcStructuralSurfaceMemberVarying_) is defined by _IfcMaterialLayerSetUsage_ and attached by the _IfcRelAssociatesMaterial.RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

The material is specified minimally by a name which corresponds with an agreed upon standardized structural material designation. An external reference to the source which specifies the material designation should be provided. Alternatively, structural material properties may be provided by means of _IfcMaterialProperties_.

In the absense of material layer set usage, direct instances of _IfcStructuralSurfaceMember_ are assumed to be located centrically relative to their reference surface. Their depth is provided in the attribute _Thickness_.

  
  
{ .use-head}
Reference Topology

The [Reference Topology](../../templates/reference-topology.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>RepresentationType</b></th><th><b>Topology</b></th></tr>
<tr><td>Face</td><td><a href="../../ifctopologyresource/lexical/ifcfacesurface.htm">IfcFaceSurface</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStructuralSurfaceMember Reference Topology</p></td></tr></table>

Direct instances of _IfcStructuralSurfaceMember_ shall have a topology representation which consists of one _IfcFaceSurface_, representing the reference surface of the surface member. See definitions at _IfcStructuralItem_ for further specifications.

The local coordinate system is established by the reference surface given by topology representation.

  
  
{ .use-head}
Structural Connectivity

The [Structural Connectivity](../../templates/structural-connectivity.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>StructuralConnection</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralcurveconnection.htm">IfcStructuralCurveConnection</a></td><td>Connections to curve members along edge(s) of surface.</td></tr>
<tr><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralsurfaceconnection.htm">IfcStructuralSurfaceConnection</a></td><td>Connections to surface members within face(s) of surface.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcStructuralSurfaceMember Structural Connectivity</p></td></tr></table>
