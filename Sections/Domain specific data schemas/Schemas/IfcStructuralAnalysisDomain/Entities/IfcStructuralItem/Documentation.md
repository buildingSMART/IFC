**Definition

from IAI:** The abstract entity_IfcStructuralItem_ covers structural members and structural connections. It defines the relation needed to associate structural actions to structural members and connections.

****Topology

Use Definition****

Instances of _IfcStructuralItem_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_".

**Local

Placement**

All _IfcStructuralItem_s which are grouped within a common _IfcStructuralAnalysisModel_ should have equal object placements. Placement within the world coordinate system of the project is the easiest way to ensure this, especially if structural items belong to more than one analysis model.

All geometric entities within the topological representation (such as _IfcVertexPoint_, _IfcEdgeCurve_, or _IfcFaceSurface_) are founded in the object coordinate system established by _ObjectPlacement_.

> <font color="#0000ff" size="-1"> HISTORY: New entity

in Release IFC2x Edition 2. </font>
>
