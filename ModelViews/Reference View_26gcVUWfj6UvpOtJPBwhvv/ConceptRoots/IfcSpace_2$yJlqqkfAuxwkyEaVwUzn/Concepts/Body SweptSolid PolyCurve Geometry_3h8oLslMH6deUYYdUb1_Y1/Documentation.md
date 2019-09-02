The following constraints apply to the 'Body' 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ and _IfcArbitraryProfileDefWithVoids_ shall be supported. The profile outline and inline curves are defined using _IfcIndexedPolyCurve_.
* **Extrusion**: The extrusion direction shall be vertically, i.e., along the positive Z Axis of the co-ordinate system of the containing spatial structure element.

Figure 1 shows an extrusion of an arbitrary profile definition with voids into the swept area solid of _IfcSpace_.

!["fig1"](../../../figures/ifcspace_standard-layout1.gif "Figure 1 &mdash; Space body swept solid")