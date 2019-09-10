**Definition from ISO/CD 10303-42:1992**: A face based surface model is described by a set of connected face sets of dimensionality 2. The connected face sets shall not intersect except at edges and vertices, except that a face in one connected face set may overlap a face in another connected face set, provided the face boundaries are identical. There shall be at least one connected face set.

A connected face set may exist independently of a surface model.

> <font color="#0000FF" size="-1">NOTE Corresponding STEP entity:
		face_based_surface_model. Please refer to ISO/IS 10303-42:1994, p. 188 for the
		final definition of the formal standard. </font>

> <font size="-1" color="#0000FF">HISTORY: New type in IFC
		Release 2x <br>ISSUE: See issue and change log for changes made in IFC Release
		2x</font>

**Informal propositions:**

1. The connected face sets shall not overlap or intersect except at common faces, edges or vertices. 
2. The fbsm faces have dimensionality 2.