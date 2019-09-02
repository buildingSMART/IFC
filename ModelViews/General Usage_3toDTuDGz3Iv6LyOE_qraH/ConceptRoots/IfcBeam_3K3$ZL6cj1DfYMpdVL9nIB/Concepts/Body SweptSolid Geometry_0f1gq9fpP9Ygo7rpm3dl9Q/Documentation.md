The following additional constraints apply to the 'SweptSolid' representation type:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Profile**: all subtypes of _IfcProfileDef_ (with exception of _IfcArbitraryOpenProfileDef_)
* **Extrusion**:&nbsp; All extrusion directions shall be supported.

Figure 1 illustrates the 'SweptSolid' geometric representation. There are no restrictions or conventions on how to use the local placement (black), solid of extrusion placement (red) and profile placement (green).

!["standard beam"](../../../figures/ifcbeam_standard-layout1.gif "Figure 1 &mdash; Beam swept solid")

Figure 2 illustrates the use of non-perpendicular extrusion to create the _IfcExtrudedAreaSolid_.

!["non-perpendicular extrusion"](../../../figures/ifcbeam_advanced-1-layout1.gif "Figure 2 &mdash; Beam non-perpendicular extrusion")