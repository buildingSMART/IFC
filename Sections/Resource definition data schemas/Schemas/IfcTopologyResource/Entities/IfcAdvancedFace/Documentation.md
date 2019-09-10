An advanced face is a specialization of a face surface that has to meet requirements on using particular topological and geometric representation items for the definition of the faces, edges and vertices.

An _IfcAdvancedFace_ is restricted to:

* have a face surface geometry of type _IfcElementarySurface_, _IfcSweptSurface_ or _IfcBSplineSurface_,
* have one _IfcFaceOuterBound_ as the bound of the face, with the exception of closed surfaces,
* have all faces to be bound by _IfcEdgeLoop_ or _IfcVertexLoop_
* have all edges to have an edge curve geometry
* have the edge curve geometry restricted to _IfcLine_, _IfcConic_, _IfcPolyline_, or _IfcBSplineCurve_

> NOTE&nbsp; Entity adapted from **advanced_face** defined in ISO 10303-511.

> HISTORY&nbsp; New entity in IFC4