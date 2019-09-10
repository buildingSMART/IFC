The _IfcConnectionSurfaceGeometry_ is used to describe the geometric constraints that facilitate the physical connection of two objects at a surface&nbsp;<font color="#0000ff">or at a face with surface geometry associated</font>. It is envisioned as a control that applies to the element connection relationships.

> <font color="#0000ff"><small>HISTORY&nbsp;
New entity in IFC Release 2x.</small><br>
  </font><small><font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp;
The provision of topology with associated geometry, <i>IfcFaceSurface</i>,
is
enabled by using the <i>IfcSurfaceOrFaceSurface</i>.</font></small>

****Geometry Use Definitions**:**

The _IfcSurface_ (or the _IfcFaceSurface_ with an associated _IfcSurface_) at the _SurfaceOnRelatingElement_ attribute defines the surface where the basic geometry items of the connected elements connects. The surface geometry and coordinates are provided within the local coordinate system of the _RelatingElement_, as specified at the _IfcRelConnectsSubtype_ that utilizes the _IfcConnectionSurfaceGeometry_. Optionally, the same&nbsp;surface geometry and coordinates can also be provided within the local coordinate system of the _RelatedElement_ by using the _SurfaceOnRelatedElement_ attribute.
