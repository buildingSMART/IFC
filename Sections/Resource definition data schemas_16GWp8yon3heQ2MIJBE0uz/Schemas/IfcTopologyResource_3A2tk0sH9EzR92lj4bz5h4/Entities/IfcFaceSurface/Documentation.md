**Definition from ISO/CD 10303-42:1992**: A face surface (IfcFaceSurface) is a subtype of face in which the geometry is defined by an associated surface. The portion of the surface used by the face shall be embeddable in the plane as an open disk, possibly with holes. However, the union of the face with the edges and vertices of its bounding loops need not be embeddable in the plane. It may, for example, cover an entire sphere or torus. As both a face and a geometric surface have defined normal directions, a BOOLEAN flag (the orientation attribute) is used to indicate whether the surface normal agrees with (TRUE) or is opposed to (FALSE) the face normal direction. The geometry associated with any component of the loops of the face shall be consistent with the surface geometry, in the sense that the domains of all the vertex points and edge curves are contained in the face geometry surface. A surface may be referenced by more than one face surface.

> <font color="#0000FF" size="-1">NOTE Corresponding STEP entity:
		  face_surface. Please refer to ISO/IS 10303-42:1994, p. 204 for the final
		  definition of the formal standard. Due to the general IFC model specification
		  rule not to use multiple inheritance, the subtype relationship to
		  geometric_representation_item is not included.</font>
> 
> <font color="#0000FF" size="-1">HISTORY New class in IFC Release 2.x
		  </font>
>

**Informal propositions**:

1. The domain of the face surface is formally defined to be the domain of its face geometry as trimmed by the loops, this domain does not include the bounding loops.
2. A face surface has non zero finite extent.
3. A face surface is a manifold.
4. A face surface is arcwise connected.
5. A face surface has surface genus 0.
6. The loops are not part of the face domain.
7. Loop geometry shall be consistent with face geometry. This implies that any edge - curves or vertex points used in defining the loops bounding the face surface shall lie on the face geometry.
8. The loops of the face shall not intersect.