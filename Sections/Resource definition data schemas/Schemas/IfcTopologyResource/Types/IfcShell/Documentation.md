**Definition from ISO/CD 10303-42:1992** This type collects together, for reference when constructing more complex models, the subtypes which have the characteristics of a shell. A shell is a connected object of fixed dimensionality d = 0; 1; or 2, typically used to bound a region. The domain of a shell, if present, includes its bounds and 0 <font face="Symbol">&pound;</font><font face="Symbol">X</font><font face="Symbol">&lt;</font><font face="Symbol">&yen;</font> .

* A shell of dimensionality 0 is represented by a graph consisting of a single vertex. The vertex shall not have any associated edges.
* A shell of dimensionality 1 is represented by a connected graph of dimensionality 1.
* A shell of dimensionality 2 is a topological entity constructed by joining faces along edges. Its domain, if present, is a connected, orientable 2-manifold with boundary, that is, a connected, oriented, finite, non-self-intersecting surface, which may be closed or open.

Shells of dimensionality 0 and 1 are not part of the current IFC release.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP type:
		shell. Please refer to ISO/IS 10303-42:1994, p. 127 for the final definition of
		the formal standard. Only the select items closed_shell (<i>IfcClosedShell</i>)
		and open_shell (<i>IfcOpenShell</i>) have been incorporated in the current IFC
		release.</font>

> <font size="-1" color="#0000FF">HISTORY: New type in IFC
		Release 2x </font>