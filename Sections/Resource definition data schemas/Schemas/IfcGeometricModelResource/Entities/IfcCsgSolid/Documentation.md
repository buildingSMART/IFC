An _IfcCsgSolid_ is the representation of a 3D shape using constructive solid geometry model. It is represented by a single 3D CSG primitive, or as a result of a Boolean operation. The operants of a Boolean operation can be Boolean operations themselves forming a CSG tree. The following volumes can be parts of the CSG tree: solid models, such as faceted B-Rep (_IfcFacetedBrep_, _IfcFacetedBrepWithVoids_), swept area solids (_IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_, _IfcSurfaceCurveSweptAreaSolid_), swept disk solids (_IfcSweptDiskSolid_), half space solids (_IfcHalfSpaceSolid_ and subtypes), and CSG primitives (subtypes of _IfcCsgPrimitive3D_).

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> A solid represented as a CSG model is defined by a collection of so-called primitive solids, combined using regularized Boolean operations. The allowed operations are intersection, union, and difference. As a special case a CSG solid can also consists of a single CSG primitive.  
>   
> A CSG solid requires two kinds of information for its complete definition: geometric and structural. > * The geometric information is conveyed by solid models. These typically primitive volumes such as cylinders, wedges and extrusions, but can include general B-Rep models. Solid models can also be half space solids.
> * The structural information is in a tree (strictly an acyclic directed graph) of Boolean result and CSG solids, which represent a &lsquo;recipe&rsquo; for building the solid. The terminal nodes are the geometric primitives and other solids. Every CSG solid has precisely one Boolean result associated with it which is the root of the tree that defines the solid. (There may be further Boolean results within the tree as operands). The significance of a CSG solid entity is that the solid defined by the associated tree is thus identified as a significant object itself, and in this way it is distinguished from other Boolean result entities representing intermediate results during the construction process.

> NOTE&nbsp; Entity adapted from **csg_solid** is defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC1.5.1