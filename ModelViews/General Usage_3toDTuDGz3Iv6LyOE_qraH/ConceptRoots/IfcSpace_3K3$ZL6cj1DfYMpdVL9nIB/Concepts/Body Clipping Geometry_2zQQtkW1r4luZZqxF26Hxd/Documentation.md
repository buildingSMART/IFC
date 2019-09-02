The following additional constraints apply to the advanced representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ is required, _IfcArbitraryProfileDefWithVoids_ shall be supported.
* **Extrusion**: The extrusion direction shall be vertically, i.e., along the positive Z Axis of the co-ordinate system of the containing spatial structure element.
* **Boolean result**: The difference operation with the second operand being of type _IfcHalfSpaceSolid_ (or one of its subtypes) shall be supported.

Figure 1 shows an extrusion of an arbitrary profile definition into the swept area solid. The solid and an half space solid are operands of the Boolean result of _IfcSpace_.

!["fig2"](../../../figures/ifcspace_advanced-layout1.gif "Figure 1 &mdash; Space body clipping")