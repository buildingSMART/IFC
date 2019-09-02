The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ is required.
* **Extrusion**: All extrusion directions shall be supported.

> NOTE&nbsp; If the wall body can be described by a vertical extrusion of a polygonal footprint with constant thickness along the axis (where vertical = into the direction of the global Z axis), the subtype _IfcWallStandardCase_ should be used. If the extrusion is not equal to global Z, then the _IfcWall_ should be used.