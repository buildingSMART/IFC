**Definition from ISO/CD 10303-42:1992**: A path is a topological entity consisting of an ordered collection of oriented edges, such that the edge start vertex of each edge coincides with the edge end of its predecessor. The path is ordered from the edge start of the first oriented edge to the edge end of the last edge. The BOOLEAN value sense in the oriented edge indicates whether the edge direction agrees with the direction of the path (TRUE) or is the opposite direction (FALSE).

An individual edge can only be referenced once by an individual path. An edge can be referenced by multiple paths. An edge can exist independently of a path.

> <font size="-1" color="#0000FF">NOTE Corresponding STEP entity: path.
		  Please refer to ISO/IS 10303-42:1994, p. 133 for the final definition of the
		  formal standard. </font>
> 
> <font size="-1" color="#0000FF">HISTORY New Entity in IFC Release
		  2.0</font>
> 


**Informal proposition**:

1. A path has dimensionality 1.
2. A path is arcwise connected.
3. The edges of the path do not intersect except at common vertices.
4. A path has a finite, non-zero extent.