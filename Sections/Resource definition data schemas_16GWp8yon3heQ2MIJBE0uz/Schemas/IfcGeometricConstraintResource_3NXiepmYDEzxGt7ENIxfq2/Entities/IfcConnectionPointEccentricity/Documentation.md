The _IfcConnectionPointEccentricity_ is used to describe the geometric constraints that facilitate the physical connection of two objects at a point or vertex point with associated point coordinates. There is a physical distance, or eccentricity, between the connection points of both object. The eccentricity can be either given by:

*  providing the _PointOnRelatingElement_and the _PointOnRelatedElement_, where both&nbsp;point coordinates are not identical within a common parent coordinate system (latestly within the world coordinate system),
* providing the _PointOnRelatingElement_and the three distance measures, _EccentricityInX_, _EccentricityInY_, and_EccentricityInZ_(or only _EccentricityInX_, and _EccentricityInY_ if the underlying coordinate system is two-dimensional), or
* providing both.

> <small>
NOTE&nbsp; If both, <i>PointOnRelatedElement</i>,
and <i>EccentricityInX</i>, <i>EccentricityInY</i>,
(<i>EccentricityInZ</i>) are provided, the values should be
consistent. In case of any non-consistency, the calculated distance
between <i>PointOnRelatingElement</i> and <i>PointOnRelatedElement</i>takes
precedence.
  </small>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in IFC 2x Edition 3.</font> </small>

****Geometry Use Definitions**:**

The _IfcPoint_ (or the _IfcVertexPoint_ with an associated _IfcPoint_) at the _PointOnRelatingElement_ attribute defines the point where the basic geometry items of the connected elements connects. The point coordinates are provided within the local coordinate system of the _RelatingElement_, as specified at the _IfcRelConnectsSubtype_ that utilizes the _IfcConnectionPointGeometry_. Optionally, the same point coordinates can also be provided within the local coordinate system of the _RelatedElement_ by using the _PointOnRelatedElement_ attribute, otherwise the distance to the point at the RelatedElement has to be given by the three eccentricity values.