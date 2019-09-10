The _IfcConnectionPointGeometry_ is used to describe the geometric constraints that facilitate the physical connection of two objects at a point (here _IfcCartesianPoint_) <font color="#0000ff">or at an vertex with point
coordinates associated</font>. It is envisioned as a control that applies to the element connection relationships.

> <small>
EXAMPLE&nbsp; The
connection relationship between two path based elements (like a column
and a beam) has a geometric constraint which describes the connection
points by a <i>PointOnRelatingElement</i> for the column
and a <i>PointOnRelatedElement</i> for the beam. The exact
usage of the <i>IfcConnectionPointGeometry</i> is further
defined in the geometry use sections of the elements that use it.<br>
  <br>
NOTE &nbsp;If the point
connection has an offset, i.e. if the two points (or vertex points) at
the relating and related element do not physically match, the subtype
IfcConnectionPointEccentricity shall be used.</small>

> <small>
  <font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 1.5, has been renamed from
IfcPointConnectionGeometry in IFC Release 2x.</font> <br>
  <font color="#ff0000">IFC2x Edition 3 CHANGE&nbsp;
The provision of topology with associated geometry, <i>IfcVertexPoint</i>, is
enabled by using the <i>IfcPointOrVertexPoint</i>.</font> </small>

****Geometry Use Definitions**:**

The _IfcPoint_ (or the _IfcVertexPoint_ with an associated _IfcPoint_) at the _PointOnRelatingElement_ attribute defines the point where the basic geometry items of the connected elements connects. The point coordinates are provided within the local coordinate system of the _RelatingElement_, as specified at the _IfcRelConnectsSubtype_ that utilizes the _IfcConnectionPointGeometry_. Optionally, the same point coordinates can also be provided within the local coordinate system of the _RelatedElement_ by using the _PointOnRelatedElement_ attribute. If both point coordinates are not identical within a common parent coordinate system (latestly within the world coordinate system), the subtype _IfcConnectionPointEccentricity_ shall be used.
