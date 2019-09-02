The _IfcConnectionCurveGeometry_ is used to describe the geometric constraints that facilitate the physical connection of two objects at a curve&nbsp;<font color="#0000ff">or at an edge with curve geometry associated</font>. It is envisioned as a control that applies to the element connection relationships.

> <small>
EXAMPLE&nbsp; The
connection relationship between two walls has a geometric constraint
which describes the end caps (or cut-off of the wall ends) by a <i>CurveOnRelatingElement</i>
for the first wall and a <i>CurveOnRelatedElement</i> for
the second wall. The exact usage of the <i>IfcConnectionCurveGeometry</i>
is further defined in the geometry use sections of the elements that
use it.</small>

The available geometry for the connection constraint may be further restricted to only allow straight segments by applying _IfcPolyline_ only. Such an usage constraint is provided at the object definition of the _IfcElement_ subtype, utilizing the element connection by referring to the subtype of _IfcRelConnects_ with the associated&nbsp;_IfcConnectionCurveGeometry._

> <small> <font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 1.5, has been renamed from
IfcLineConnectionGeometry in IFC Release 2x.<br>
  </font></small><small><font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp;
The provision of topology with associated geometry, <i>IfcEdgeCurve</i>,
is
enabled by using the <i>IfcCurveOrEdgeCurve</i>.</font></small>

****Geometry Use Definitions**:**

The _IfcCurve_ (or the _IfcEdgeCurve_ with an associated _IfcCurve_) at the _CurveOnRelatingElement_ attribute defines the curve where the basic geometry items of the connected elements connects. The curve geometry and coordinates are provided within the local coordinate system of the _RelatingElement_, as specified at the _IfcRelConnects_Subtype that utilizes the _IfcConnectionCurveGeometry_. Optionally, the same curve geometry and coordinates can also be provided within the local coordinate system of the _RelatedElement_ by using the _CurveOnRelatedElement_ attribute.