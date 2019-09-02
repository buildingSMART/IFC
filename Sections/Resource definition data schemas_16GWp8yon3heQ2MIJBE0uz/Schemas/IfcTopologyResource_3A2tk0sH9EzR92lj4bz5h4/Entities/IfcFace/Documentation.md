**Definition from ISO/CD 10303-42:1992**: A face is a topological entity of dimensionality 2 corresponding to the intuitive notion of a piece of surface bounded by loops. Its domain, if present, is an oriented, connected, finite 2-manifold in _R^m^_. A face domain shall not have handles but it may have holes, each hole bounded by a loop. The domain of the underlying geometry of the face, if present, does not contain its bounds, and 0 &lt; &Xi; &lt; &infin;.

A face is represented by its bounding loops, which are defined as face bounds. A face has a topological normal n and the tangent to a loop is t. For a loop bounding a face with defined geometry, the cross product n x t points toward the interior of the face. That is, each loop runs counter-clockwise around the face when viewed from above, if we consider the normal n to point up. With each loop is associated a BOOLEAN flag to signify whether the loop direction is oriented with respect to the face normal (TRUE) or should be reversed (FALSE).

A face shall have at least one bound, and the loops shall not intersect. One loop is optionally distinguished as the outer loop of the face. If so, it establishes a preferred way of embedding the face domain in the plane, in which the other bounding loops of the face are inside the outer bound. Because the face domain is arcwise connected, no inner loop will contain any other loop. This is true regardless of which embedding in the plane is chosen.

The edges and vertices referenced by the loops of a face form a graph, of which the individual loops are the connected components. The Euler equation (1) for this graph becomes:

> 
>> ![Image](figures/IfcFace-Math1.gif)
>>


> 
where _G^l^~i~_ is the graph genus of the_i_^th^ loop.

> <font color="#0000FF" size="-1"><font color="#0000FF" size="-1">NOTE
		  Corresponding STEP entity: face. No subtypes of face have been incorporated
		  into this IFC Release. Please refer to ISO/IS 10303-42:1994, p. 140 for the
		  final definition of the formal standard. The WR1 has not been incorporated,
		  since it is always satisfied, due to the fact that only poly loops exist for
		  face bounds. </font></font>
> 
> <font color="#0000FF" size="-1">HISTORY New class in IFC Release 1.0
		  </font>
>

**Informal propositions**:

1. No edge shall be referenced by the face more than twice. 
2. Distinct face bounds of the face shall have no common vertices. 
3. If geometry is present, distinct loops of the same face shall not intersect. 
4. The face shall satisfy the Euler Equation: (number of vertices) - (number of edges) - (number of loops) + (sum of genus for loops) = 0.