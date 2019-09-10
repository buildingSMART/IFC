**Definition
from IAI:** The entity _IfcBoundaryFaceCondition_ describes boundary conditions that can be applied to structural face connections, either directly for the connection (e.g. the connecting face) or for the relation between a structural member and the connection.

The following conventions to the values of the _LinearStiffnessByArea[X,Y,Z]_ apply:

* value (-1.) represents an infinitive large value &ndash; or a fixed connectivity with infinitive stiffness
* value zero (0.), represents no stiffness or a free connectivity
* any other value represents a finitive stiffness or spring connectivity in that direction or rotation
* value NIL ($) represents an unknown connectivity condition

> <font size="-1">NOTE: Instances of the entity <i>IfcBoundaryFaceCondition</i>
are used e.g., to define the boundary condition for instances of <i>IfcStructuralFaceConnection</i>
or <i>IfcRelConnectsStructuralMember</i>
pointing to a structural face connection. </font>

> <font color="#0000ff" size="-1">HISTORY: New entity
in Release IFC2x edition 2. </font>
>
