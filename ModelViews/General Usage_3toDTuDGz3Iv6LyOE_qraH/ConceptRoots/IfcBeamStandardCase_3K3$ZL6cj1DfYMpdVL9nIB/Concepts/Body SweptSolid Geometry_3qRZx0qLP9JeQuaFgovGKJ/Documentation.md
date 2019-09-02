The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
* **Solid Position** : The _IfcSweptAreaSolid.Position_ shall exclusively been used to correspond to the cardinal point. The x/y offset of the _Position_ represents the cardinal point offset of the profile against the axis. No rotation shall be allowed.
* **Profile**: All subtypes of _IfcParameterizedProfileDef_
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.
* **Extrusion**:&nbsp;Perpendicular to the profile direction. The _IfcExtrudedAreaSolid.ExtrudedDirection_ shall be [0.,0.,1.].
* **Orientation**: The y-axis of the profile, as determined by _IfcSweptAreaSolid.Position.P[2]_ shall point upwards. It indicates the "role" of the beam, a role=0&deg; means y-axis of profile pointing upwards.

Figure 1 illustrates a standard geometric representation with cardinal point applied as **1** (bottom left).

The following interpretation of dimension parameter applies for rectangular beams with linear extrusions:

* _IfcRectangleProfileDef.YDim_ interpreted as beam height
* _IfcRectangleProfileDef.XDim_ interpreted as beam width

The following interpretation of dimension parameter applies for circular beams:

* _IfcCircleProfileDef.Radius_ interpreted as beam radius.

!["standard beam"](../../../figures/ifcbeamstandardcase_sweptsolid-01.png "Figure 1 &mdash; Beam body extrusion")