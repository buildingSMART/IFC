The following additional constraints apply to the 'SweptSolid' representation type:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcRectangleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded in any direction relative to the XY plane of the position coordinate system of the _IfcExtrudedAreaSolid_. Therefore non-perpendicular sweep operation has to be supported. It might be further constrained to be in the direction of the global z-axis in implementers agreements.

Figure 1 illustrates the body representation.

!["fig1"](../../../figures/IfcRampFlight-Layout1.gif "Figure 1 &mdash; Ramp flight body")