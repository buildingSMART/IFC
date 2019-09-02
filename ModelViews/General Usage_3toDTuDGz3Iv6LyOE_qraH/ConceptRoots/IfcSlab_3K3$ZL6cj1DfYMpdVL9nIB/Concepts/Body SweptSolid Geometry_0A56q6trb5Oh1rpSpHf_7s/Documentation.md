The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcRectangleProfileDef, IfcCircleProfileDef, IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.

Figure 1 illustrates a 'SweptSolid' geometric representation.

> NOTE&nbsp; The following interpretation of dimension parameter applies for polygonal slabs (in ground floor view): > * _IfcArbitraryClosedProfileDef.OuterCurve_: closed bounded curve interpreted as area (or foot print) of the slab.

!["standard slab"](../../../figures/ifcslab_standard-layout1.gif "Figure 1 &mdash; Slab body extrusion")