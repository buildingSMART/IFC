The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Profile**: all subtypes of _IfcProfileDef_ (with exception of _IfcArbitraryOpenProfileDef_) 
* **Extrusion**: All extrusion directions shall be supported

Figure 1 illustrates a 'SweptSolid' geometric representation. There are no restrictions or conventions on how to use the local placement (black), solid of extrusion placement (red) and profile placement (green).

!["standard column"](../../../figures/ifccolumn_standard-layout1.gif "Figure 1 &mdash; Column swept solid")

Figure 2 illustrates use of a special profile type (here _IfcIShapeProfileDef_) for the definition of the _IfcExtrudedAreaSolid_.

!["advanced column"](../../../figures/ifccolumn_advanced-1-layout1.png "Figure 2 &mdash; Column extrusion of I-Shape")