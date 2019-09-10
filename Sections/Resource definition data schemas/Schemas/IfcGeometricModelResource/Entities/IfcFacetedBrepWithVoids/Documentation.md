The _IfcFacetedBrepWithVoids_ is a specialization of a faceted B-rep which contains one or more voids in its interior. The voids are represented as closed shells which are defined so that the shell normal point into the void.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  brep_with_voids (see note above). Please refer to ISO/IS 10303-42:1994, p. 173
		  for the final definition of the formal standard. In IFC faceted B-rep with
		  voids is represented by this subtype <i>IfcFacetedBrepWithVoids</i> and not
		  defined via an implicit ANDOR supertype constraint as in ISO/IS 10303-42:1994
		  between an instance of faceted_brep AND brep_with_voids. This change has been
		  made due to the fact, that only ONEOF supertype constraint is allowed within
		  the IFC object model. </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 1.0
		  </font>
>

**Informal propositions:**

1. Each void shell shall be disjoint from the outer shell and from every other void shell 
2. Each void shell shall be enclosed within the outer shell but not within any other void shell. In particular the outer shell is not in the set of void shells 
3. Each shell in the _IfcManifoldSolidBrep_ shall be referenced only once. 
4. All the bounding loops of all the faces of all the shells in the _IfcFacetedBrep_ shall be of type _IfcPolyLoop_.