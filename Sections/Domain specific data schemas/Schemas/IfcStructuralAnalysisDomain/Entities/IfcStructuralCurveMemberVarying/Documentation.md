**Definition
from IAI:** Instances of the entity _IfcStructuralCurveMemberVarying_ shall be used to describe linear structural elements with varying profile properties.

The varying profile properties are assigned through the _IfcRelAssociatesProfileProperties_ with an additional link to the _IfcShapeAspect_, which relates the profile properties to the different vertices of the structural curve member.

> <font color="#0000ff" size="-1"> HISTORY: New entity
in Release IFC2x Edition 2. </font>
> 


****Use
Definition****

<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td><img alt="fig 1" src="figures/ifcstructuralcurvemembervarying-fig1.gif" height="525" width="632"></td>
      <td valign="top">The
varying profiles along the longitudinal axis are assigned by using
several relationships of <i>IfcRelAssociatesProfileProperties</i>,
each assigning one profile definition (<i>IfcProfileProperties</i>
optionally referencing one <i>IfcProfileDef</i>)
to a vertex along the longitudinal axis.<br>
      <br>
The topological representation is an <i>IfcEdge</i>,
decomposed into <i>IfcSubEdge</i>'s,
a changing profile definition is associated to the start or end vertex
of the <i>IfcSubEdge</i>.</td>
    </tr>
  </tbody>
</table>

****Topology
Use Definition****

Instances of _IfcStructuralCurveMemberVarying_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_".

The guidelines on using the location and topological representation capabilities are identical with the supertype _IfcStructuralCurveMember_. The additional requirement is that if the varying profile not only has different (morphing) profiles at the start and end edge, then the _IfcTopologyRepresentation.Item[1]_shall be an _IfcEdge_ (or _IfcEdgeCurve_, _IfcOrientedEdge_) that is referenced by the _Parent_ attribute of at least two _IfcSubedge_'s.

****Shape
Aspect Use Definition****

The attribute _HasAssociations_ references a set of _IfcRelAssociatesProfileProperties_, each referring to an _IfcShapeAspect_, that has a list of _ShapeRepresentations_. Each individual _IfcShapeRepresentation_ within that list shall have a single (or two) item(s) within its list of _Items_. The type of the item shall be:

* _IfcVertexPoint_

It references either a start or an end vertex (or both) to which the profile properties apply.
