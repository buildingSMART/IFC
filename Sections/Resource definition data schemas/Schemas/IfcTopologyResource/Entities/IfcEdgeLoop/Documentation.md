**Definition from ISO/CD 10303-42:1992**: An edge_loop is a loop with nonzero extent. It is a path in which the start and end vertices are the same. Its domain, if present, is a closed curve. An edge_loop may overlap itself.

Informal propositions:

1. The genus of the _IfcEdgeLoop_ shall be 1 or greater.
2. The Euler formula shall be satisfied:  (number of vertices) + genus - (number of edges) = 1;
3. No edge may be referenced more than once by the same _IfcEdgeLoop_ with the same sense. For this purpose, an edge which is not an oriented edge is considered to be referenced with the sense TRUE.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  edge_loop. Please refer to ISO/IS 10303-42:1994, p. 122 for the final
		  definition of the formal standard. </font>
> 
> <font color="#0000FF" size="-1"> HISTORY: New Entity in Release IFC 2x
		  Edition 2. </font>
>
