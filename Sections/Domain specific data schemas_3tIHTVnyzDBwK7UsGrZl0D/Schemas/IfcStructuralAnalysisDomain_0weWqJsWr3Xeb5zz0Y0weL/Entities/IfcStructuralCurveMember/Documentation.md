**Definition
from IAI:** Instances of the entity _IfcStructuralCurveMember_ shall be used to describe linear structural elements. Profile and material properties are defined by using objectified relationships:

* The material properties are defined by _IfcMechanicalMaterialProperties_ (and subtypes), they are connected through _IfcMaterial_ and _IfcRelAssociatesMaterial_ and are accessible via the inherited inverse relationship _HasAssociations_.
* The profile properties are defined by _IfcMechanicalProfileProperties_ (and subtypes), they are connected through _IfcRelAssociatesProfileProperties_ and are accessible via the inherited inverse relationship _HasAssociations_.

> <font color="#0000ff" size="-1"> HISTORY: New entity
in Release
IFC2x Edition 2. </font>
> 


****Use
Definition****

<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td><img alt="curve member" src="figures/IfcStructuralCurveMember-Fig1.gif" height="380" width="580"><br>
      </td>
      <td valign="top">The
topological (or axis) representation of the
structural curve member is given by assigning an edge through the
general <i>Representation</i>
capability inherited by <i>IfcProduct</i>.<br>
      <br>
For linear structural curve members the use of <i>IfcEdge</i>
is
sufficient, since a linear interpolation between the two vertices is
assumed, if the structural curve member is an arc, or other non-linear
form, the <i>IfcEdgeCurve</i>
needs to be used instead, having the
geometric form of the curve between the two vertices fully defined.<br>
      <br>
A single, constant, profile definition is assigned to the structural
curve member through the <i>IfcRelAssociatedProfileProperties</i>.</td>
    </tr>
  </tbody>
</table>

****Topology
Use Definition****

Instances of _IfcStructuralCurveMember_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_".

**Placement**

The placement for _IfcStructuralCurveMember_ is determined at its supertype _IfcProduct_. It is defined by the optional _IfcObjectPlacement_, referenced by _ObjectPlacement_ at _IfcProduct_, which establishes, if given, the object coordinate system that is referenced by all topological representations of that product.

* If the _ObjectPlacement_ attribute is omitted, then all topological representations are given directly in world coordinates. This is the preferred representation.
* If the _ObjectPlacement_ attribute is provided, then it establishes an object coordinate system for all topological representations which are given object coordinates. 
    * If the _PlacementRelTo_ relationship of _IfcLocalPlacement_ is omitted, the object coordinate system is established within the world coordinate system.
    * If the _PlacementRelTo_ relationship of _IfcLocalPlacement_ is given, it shall point to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that.  

**Topology
Representation**

Instances of _IfcStructuralCurveMember_ shall have a topology representation given by an edge with an optional additional geometric representation of the included curve. It can be provided by either

* _IfcEdge_
* _IfcOrientedEdge_
* _IfcEdgeCurve_

which should be the single item of _IfcTopologyRepresentation.Items_. The _IfcEdge_ might be referenced by two or many _IfcSubedge_, representing sections of the _IfcStructuralCurveMember_ with changing properties. See subtype _IfcStructuralCurveMemberVarying_ for the use definition.