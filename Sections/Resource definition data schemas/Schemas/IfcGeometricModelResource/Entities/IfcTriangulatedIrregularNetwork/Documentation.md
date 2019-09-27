﻿The _IfcTriangulatedIrregularNetwork_ is a triangulated face set for representing horizontal surfaces (one unique Z coordinate for all X and Y coordinates within domain) with additional flags for each face indicating breaklines between faces or designation as a hole or void. Triangles shall be defined with vertices in counterclockwise order as viewing from above (following right-hand rule).

For visualization, applications should not display faces where flags are set as negative (either a hole, void, or possible future extension).

The flag _Void_ shall be used to indicate that faces are to be excluded without falling back on any other geometry. Such designation could be used for portions of a site beneath a building or other structure.

The flag _Hole_ shall be used to indicate that faces are to be excluded but may fall back on other geometry. Such designation could be used for portions of a proposed site that are to remain unchanged (conforming to an existing site that may also be defined)

For scenarios where multiple surfaces used as input are to be combined, any triangles marked _Void_ shall be retained as voids, while any triangles marked as _Hole_ shall be overridden if another surface has visible geometry defined within the same horizontal location.
