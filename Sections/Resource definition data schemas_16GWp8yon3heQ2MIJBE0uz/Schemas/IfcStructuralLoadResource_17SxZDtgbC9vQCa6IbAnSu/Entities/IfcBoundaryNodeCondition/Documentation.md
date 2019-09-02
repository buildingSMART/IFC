**Definition
from IAI:** The entity _IfcBoundaryNodeCondition_ describes boundary conditions that can be applied to structural point connections, either directly for the connection (e.g. the joint) or for the relation between a structural member and the connection.&nbsp;

The following conventions to the values of the _LinearStiffness[X,Y,Z]_ and _RotationalStiffness[X,Y,Z]_ apply:

* value (-1.) represents an infinitely large value &ndash; or a fixed connectivity with infinitive stiffness
* value zero (0.), represents no stiffness or a free connectivity
* any other value represents a finitive stiffness or spring connectivity in that direction or rotation
* value NIL ($) represents an unknown connectivity condition

> <font size="-1">NOTE: Instances of the entity <i>IfcBoundaryNodeCondition</i>
are used e.g., to define the boundary condition for instances of <i>IfcStructuralPointConnection</i>
or <i>IfcRelConnectsStructuralMember</i>
pointing to a structural node connection.</font>

> <font color="#0000ff" size="-1">HISTORY: New entity
in Release IFC2x Edition 2. </font>
>