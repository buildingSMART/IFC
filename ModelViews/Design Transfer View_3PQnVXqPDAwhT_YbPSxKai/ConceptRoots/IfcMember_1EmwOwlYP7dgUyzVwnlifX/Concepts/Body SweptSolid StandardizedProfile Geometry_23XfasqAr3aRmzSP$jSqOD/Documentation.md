The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Profile**: All subtypes of _IfcParameterizedProfileDef_
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.
* **Extrusion**: perpendicular to the profile direction.
* **Orientation**: The y-axis of the profile, as determined by _IfcSweptAreaSolid.Position.P[2]_ shall point to the Z-Axis. It indicates the "role" of the column, a role=0&deg; means y-axis of profile = Z-axis of reference coordinate system. In the exception of a vertical member, the y-axis shall point to the Y-axis.

Figure 1 illustrates a 'SweptSolid' geometric representation with cardinal point applied as **1** (bottom left).

The following interpretation of dimension parameter applies for rectangular members:

* <small><em>IfcRectangleProfileDef.YDim</em> interpreted as member width</small>
* <small><em>IfcRectangleProfileDef.XDim</em> interpreted as member depth</small>

The following interpretation of dimension parameter applies for circular members:

* <small><em>IfcCircleProfileDef.Radius</em> interpreted as beam radius.</small>

!["standard member"](../../../figures/ifcbeamstandardcase_sweptsolid-01.png "Figure 1 &mdash; Member body extrusion")