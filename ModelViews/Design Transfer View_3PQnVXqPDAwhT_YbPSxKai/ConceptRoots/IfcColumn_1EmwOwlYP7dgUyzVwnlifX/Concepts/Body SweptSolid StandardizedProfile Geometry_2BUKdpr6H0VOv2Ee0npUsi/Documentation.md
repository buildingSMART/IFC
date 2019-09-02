The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Profile**: All subtypes of _IfcParameterizedProfileDef_
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.
* **Extrusion**: perpendicular to the profile direction. The _IfcExtrudedAreaSolid.ExtrudedDirection_ shall be [0.,0.,1.].
* **Orientation**: The y-axis of the profile, as determined by _IfcSweptAreaSolid.Position.P[2]_ shall point to the Y-Axis. It indicates the "role" of the column, a role=0&deg; means y-axis of profile = Y-axis of reference coordinate system.

Figure 1 illustrates a standard geometric representation with cardinal point applied as **5** (mid-depth centre).

The following interpretation of dimension parameter applies for rectangular columns:

* _IfcRectangleProfileDef.YDim_ interpreted as column width
* _IfcRectangleProfileDef.XDim_ interpreted as column depth

The following interpretation of dimension parameter applies for circular columns:

* _IfcCircleProfileDef.Radius_ interpreted as column radius.

!["standard column"](../../../figures/ifccolumnstandardcase_sweptsolid-01.png "Figure 1 &mdash; Column body extrusion")