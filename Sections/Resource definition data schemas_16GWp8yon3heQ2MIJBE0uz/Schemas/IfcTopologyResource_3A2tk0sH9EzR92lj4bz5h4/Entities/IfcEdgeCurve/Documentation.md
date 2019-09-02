**Definition from ISO/CD 10303-42:1992**: An edge curve is a special subtype of edge which has its geometry fully defined. The geometry is defined by associating the edge with a curve which may be unbounded. As the topological and geometric directions may be opposed, an indicator (same sense) is used to identify whether the edge and curve directions agree or are opposed. The Boolean value indicates whether the curve direction agrees with (TRUE) or is in the opposite direction (FALSE) to the edge direction. Any geometry associated with the vertices of the edge shall be consistent with the edge geometry.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  edge_curve. Please refer to ISO/IS 10303-42:1994, p. 132 for the final
		  definition of the formal standard. Due to the general IFC model specification
		  rule not to use multiple inheritance, the subtype relationship to
		  geometric_representation_item is not included.</font>
> 
> <font color="#0000FF" size="-1"> HISTORY: New Entity in IFC Release
		  2.x. </font>
>

**Informal propositions**:

1. The domain of the edge curve is formally defined to be the domain of its edge geometry as trimmed by the vertices. This domain does not include the vertices.
2. An edge curve has non-zero finite extent.
3. An edge curve is a manifold.
4. An edge curve is arcwise connected.
5. The edge start is not a part of the edge domain.
6. The edge end is not a part of the edge domain.
7. Vertex geometry shall be consistent with edge geometry.