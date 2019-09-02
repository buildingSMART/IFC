_IfcConnectionPointGeometry_ is used to describe the geometric constraints that facilitate the physical connection of two objects at a point (here _IfcCartesianPoint_) or at an vertex with point coordinates associated. It is envisioned as a control that applies to the element connection relationships.

> EXAMPLE&nbsp; The connection relationship between two path based elements (like a column and a beam) has a geometric constraint which describes the connection points by a _PointOnRelatingElement_ for the column and a _PointOnRelatedElement_ for the beam. The exact usage of the _IfcConnectionPointGeometry_ is further defined in the geometry use sections of the elements that use it.

The _IfcPoint_ (or the _IfcVertexPoint_ with an associated _IfcPoint_) at the _PointOnRelatingElement_ attribute defines the point where the basic geometry items of the connected elements connect. The point coordinates are provided within the local coordinate system of the _RelatingElement_, as specified at the _IfcRelConnectsSubtype_ that utilizes the _IfcConnectionPointGeometry_. Optionally, the same point coordinates can also be provided within the local coordinate system of the _RelatedElement_ by using the _PointOnRelatedElement_ attribute. If both point coordinates are not identical within a common parent coordinate system (ultimately within the world coordinate system), the subtype _IfcConnectionPointEccentricity_ shall be used.

> NOTE&nbsp; If the point connection has an offset (if the two points or vertex points at the relating and related element do not physically match), the subtype _IfcConnectionPointEccentricity_ shall be used.

> HISTORY&nbsp; New entity in IFC1.5.

{ .change-ifc2x}
> IFC2x CHANGE&nbsp; Renamed from IfcPointConnectionGeometry.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The provision of topology with associated geometry, _IfcVertexPoint_, is enabled by using the _IfcPointOrVertexPoint_.