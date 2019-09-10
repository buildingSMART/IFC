The schema _IfcGeometricModelResource_ defines the resources used for geometric model representations. The primary application of this resource is for representation of the shape or geometric form of a product model.

> <font color="#0000FF">NOTE: The definitions of this resource of
		the IFC model have been taken from the Integrated Resource, part 42 "Integrated
		generic resources: Geometric and topological representations" of the ISO
		standard 10303: "Industrial automation systems and integration - Product data
		representation and exchange". The IfcGeometricModelResource refers to the
		clause 6, "Geometric Model" of the standard. The reference is ISO/IS
		10303-42:1994, pp. 166. The improved definitions of the second edition, ISO/DIS
		10303-42:1999 have been used, when applicable.</font>

The definitions taken from ISO/IS 10303-42:1994 have undergone a adaptation process, characterized by:

* adaptation of the IFC naming convention (inner majuscules and Ifc prefix)
* adaptation of the STEP entities, where multiple inheritance or non-exclusive inheritance (i.e. AND or ANDOR subtype constraints) are used
* selection of a subset of the IR, using subtype and select pruning
* dimensionality of geometric representation items defined at each item (not through the representation context)
* omission of the name attribute at the representation item
* using profile definitions instead of curve bounded surface for the swept surface of swept area solid
* restriction of the manifold solid brep to support faceted breps only
* additional subtype of half space solid added
* additional constraining subtype of Boolean result added

The geometric representation of the shape is defined following the adaptation of the **ISO/CD 10303-42:1992**, _Industrial Automation Systems
		and Integration: Product Data Representation and Exchange - Part 42: Integrated
		Generic Resources. Geometric and Topological Representation_. The type, class, and function semantic definition sections follow the adapted wording of the working draft, which is clearly indicated and quoted at each reference. The definitions on geometric and topological representation (when taken from ISO/CD 10303-42:1992) are explicitly excluded from the copyright of the International Alliance of Interoperability.

> <font color="#0000FF">For more information on the definitions
		as defined in the formal ISO standard please refer to: ISO/IS 10303-42:1994,
		Industrial Automation Systems and Integration: Product Data Representation and
		Exchange - Part 42: Integrated Generic Resources. Geometric and Topological
		Representation. The formal standard can be obtained through the local
		publishers of standards in each individual country.</font>

The following is within the scope of the geometric model representation in the current version of the geometric model resource:

* data describing the precise geometric form of three-dimensional solid objects;
* constructive solid geometry (CSG) models;
* definition of half-spaces (CSG primitives are not in scope);
* creation of solid models by sweeping operations (swept area solids only);
* manifold boundary representation (brep) models (restricted to faceted brep);
* surface models;
* geometric sets.

### Fundamental Concepts and Assumptions
> <font color="#0000FF">NOTE: The following fundamental concepts
		and assumptions are taken from ISO/CD 10303-42:1992. Please refer to ISO/IS
		10303-42:1994, pp.166-167 for the final definition of the formal
		standard.</font>

> <font color="#0000FF">NOTE: Only the parts relevant to the
		subset of ISO 10303-42 (which had been incorporated into the
		IfcGeometricModelResource) are quoted.</font>

The constructive solid geometry models are represented by their component primitives and the sequence of Boolean operations (union, intersection, or difference) used in their construction. The entity which communicates the logical sequence of Boolean operations is the boolean result (_IfcBooleanResult_) which identifies an operator and two operands. Since the operands can themselves be Boolean results thus enabling nested operations. Swept solids and half-space solids are permissible Boolean operands. The swept solids are the solid of revolution and the solid of linear extrusion. The swept solids are obtained by extruding or sweeping a planar face which may contain holes. The half space solid is essentially defined as a semi-infinite solid on one side of a surface; it may be limited by a box domain.

Brep models are represented by the set of shells defining the exterior or interior boundaries. The faceted brep is restricted to represent breps in which all faces are planar and every loop is a poly loop. For such a solid this entity provides a more efficient form of representation. The shell based surface model, the face based surface model and the geometric set entities do not enforce the integrity checks of the manifold solid brep and can be used for the communication of incomplete models (including two-dimensional models).