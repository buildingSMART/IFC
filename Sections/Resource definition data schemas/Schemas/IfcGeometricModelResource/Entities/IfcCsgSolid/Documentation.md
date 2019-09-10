**Definition from ISO/CD 10303-42:1992**: A solid represented as a CSG model is defined by a collection of so-called primitive solids, combined using regularized Boolean operations. The allowed operations are intersection, union, and difference. As a special case a CSG solid can also consists of a single CSG primitive.

*  A CSG solid requires two kinds of information for its complete definition: geometric and structural. The geometric information is conveyed by solid models. These typically primitive volumes such as cylinders, wedges and extrusions, but can include general B-Rep models. There can also be solid replicas (not in current IFC release) and half space solids. 
* The structural information is in a tree (strictly an acyclic directed graph) of Boolean result and CSG solids, which represent a &#145;recipe&#146; for building the solid. The terminal nodes are the geometric primitives and other solids. Every CSG solid has precisely one Boolean result associated with it which is the root of the tree that defines the solid. (There may be further Boolean results within the tree as operands). The significance of a CSG solid entity is that the solid defined by the associated tree is thus identified as a significant object itself, and in this way it is distinguished from other Boolean result entities representing intermediate results during the construction process. 

The following primitive volumes can be parts of the CSG tree: solid models, i.e. faceted B-Rep (_IfcFacetedBrep,
		IfcFacetedBrepWithVoids_), swept area solid (_IfcExtrudedAreaSolid,
		IfcRevolvedAreaSolid, IfcSurfaceCurveSweptAreaSolid_), swept disk solids (_IfcSweptDiskSolid_) and half space solids (_IfcHalfSpaceSolid_and subtypes). CSG primitives are out of scope for current IFC Release.

> <font color="#0000FF" size="-1">NOTE Corresponding STEP entity:
		  csg_solid, please refer to ISO/IS 10303-42:1994, p.174 for the final definition
		  of the formal standard. </font>
> 
> <font color="#0000FF" size="-1">HISTORY New class in IFC Release 1.5.1
		  </font>
>
