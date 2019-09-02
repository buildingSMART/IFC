{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> An edge_loop is a loop with nonzero extent. It is a path in which the start and end vertices are the same. Its domain, if present, is a closed curve. An edge_loop may overlap itself.

> NOTE&nbsp; Entity adapted from **edge_loop** defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC2x2.

{ .spec-head}
Informal Propositions:

1. The genus of the _IfcEdgeLoop_ shall be 1 or greater.
2. The Euler formula shall be satisfied:  (number of vertices) + genus - (number of edges) = 1;
3. No edge may be referenced more than once by the same _IfcEdgeLoop_ with the same sense. For this purpose, an edge which is not an oriented edge is considered to be referenced with the sense TRUE.