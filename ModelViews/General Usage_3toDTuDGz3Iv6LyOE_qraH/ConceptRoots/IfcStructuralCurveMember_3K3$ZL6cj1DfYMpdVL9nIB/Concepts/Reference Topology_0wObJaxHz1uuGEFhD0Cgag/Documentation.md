Direct instances of _IfcStructuralCurveMember_ shall have a topology representation which consists of one instance of _IfcEdge_ or a subtype, representing the reference curve of the curve member. See definitions at _IfcStructuralItem_ for further specifications.

{ .spec-head}
Informal Propositions:

1. The reference curve must not be parallel with _Axis_ at any point within the curve member's domain.

The local coordinate system is established by the reference curve given by topology representation and by the attribute _Axis_. The local x axis is parallel with the tangent on the reference curve. The local z axis is located in the surface which is created by sweeping _Axis_ along the reference curve and is directed according to _Axis_. The local y axis is directed such that x,y,z form a right-handed Cartesian coordinate system.