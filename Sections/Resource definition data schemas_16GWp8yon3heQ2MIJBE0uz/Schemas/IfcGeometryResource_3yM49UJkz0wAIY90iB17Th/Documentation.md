The schema _IfcGeometryResource_ defines the resources used for geometric representations. The primary application of this resource is for representation of the shape or geometric form of a product model.

> <font color="#0000FF">NOTE: The definitions of this resource of
		the IFC model have been taken from the Integrated Resource, part 42 "Integrated
		generic resources: Geometric and topological representations" of the ISO
		standard 10303: "Industrial automation systems and integration - Product data
		representation and exchange". The IfcGeometryResource refers to the clause 4,
		"Geometry" of the standard. The reference is ISO/IS 10303-42:1994, p. 11-121.
		The improved definitions of the second edition, ISO/DIS 10303-42:1999 have been
		used, when applicable.</font>

The definitions taken from ISO/IS 10303-42:1994 have undergone a adaptation process, characterized by:

* adaptation of the IFC naming convention (inner majuscules and Ifc prefix)
* adaptation of the STEP entities, where multiple inheritance or non-exclusive inheritance (i.e. AND or ANDOR subtype constraints) are used
* selection of a subset of the IR, using subtype and select pruning
* dimensionality of geometric representation items defined at each item (not through the representation context)
* omission of pcurves, use of simple 2D curves for the generation of swept surfaces
* omission of the name attribute at the representation item

The following entities, defined in the Integrated Resources, part 43 "Integrated generic resources: Representation structures" have been incorporated in this resource schema:

* representation_item as IfcRepresentationItem
* representation_map as IfcRepresentationMap
* mapped_item as IfcMappedItem

The geometric representation of the shape is defined following the adaptation of the **ISO/CD 10303-42:1992**, _Industrial Automation Systems
		and Integration: Product Data Representation and Exchange - Part 42: Integrated
		Generic Resources. Geometric and Topological Representation_. The type, class, and function semantic definition sections follow the adapted wording of the working draft, which is clearly indicated and quoted at each reference. The definitions on geometric and topological representation (when taken from ISO/CD 10303-42:1992) are explicitly excluded from the copyright of the International Alliance of Interoperability.

> <font color="#0000FF">For more information on the definitions
		as defined in the formal ISO standard please refer to: ISO/IS 10303-42:1994,
		Industrial Automation Systems and Integration: Product Data Representation and
		Exchange - Part 42: Integrated Generic Resources. Geometric and Topological
		Representation. The formal standard can be obtained through the local
		publishers of standards in each individual country.</font>

The following is within the scope of the geometric representation in the current version of the geometry resource:

* definition of points directly by their coordinate values
* definition of directions, vectors, and axis placements 
* definition of transformation operators
* definition of parametric curves (subset of) 
*  definition of conic curves and elementary surfaces (subset of) 
*  definition of curves defined on a parametric surface (adapted subset of) 
* definition of swept surfaces (adapted subset of)
* definition of offset curves

### Definitions
> <font color="#0000FF">NOTE: The following definitions are taken
		from ISO/CD 10303-42:1992. Please refer to ISO/IS 10303-42:1994, p. 3-7 for the
		final definition of the formal standard.</font>

**placement coordinate system:**  
a rectangular Cartesian coordinate system associated with the placement of a geometric entity in space, used to describe the interpretation of the attributes and to associate a unique parameterization with curve and surface entities."

### Fundamental concepts and assumptions
> <font color="#0000FF">NOTE: The following fundamental concepts
		and assumptions are taken from ISO/CD 10303-42:1992. Please refer to ISO/IS
		10303-42:1994, p. 12-14 for the final definition of the formal
		standard.</font>

> <font color="#0000FF">NOTE: Only the parts relevant to the
		subset of ISO 10303-42 (which had been incorporated into the
		IfcGeometryResource) are quoted.</font>

**Space Dimensionality**  
All geometry shall be defined in a right-handed rectangular Cartesian coordinate system with the same units on each axis. A common scheme has been used for the definition of both two-dimensional and three-dimensional geometry. Points and directions exists in both a two-dimensional and a three-dimensional form, these forms are distinguished solely by the presence, or absence, of a third coordinate value. Complex geometric entities are all defined using points and directions from which their space dimensionality can be deduced.

**Parameterization of analytic curves and surfaces**  
Each curve on surface specified here has a defined parameterization. In some instances the definitions are in parametric terms. In others, the conic curves and elementary surfaces, the definitions are in geometric terms. In this latter case a placement coordinate system is used to define the parameterization. The geometric definitions contain some, but not all, of the data required for this. The relevant data to define this placement coordinate system is contained in the axis2_placement (IfcAxis2Placement) associated with the individual curve and surface entities.

**Curves**  
The curve entities include lines, some elementary conics, and some referentially or procedurally defined curves. All the curves have a well defined parameterization which makes it possible to trim a curve or identify points on the curve by parameter value. For the conic curves a method of representation is used which separates their geometric form from their orientation and position in space. In each case, the position and orientation information is conveyed by an axis2_placement (IfcAxis2Placement). A composite curve entity, which includes the facility to communicate continuity information at the curve-to-curve transition points, is provided for the construction of more complex curves. The offset curve type is a curve defined with reference to other geometry. Separate offset curves entities exist for 2D and 3D applications.

**Surfaces**  
The simple surfaces are the planar surface, a surface of revolution and a surface of linear extrusion. As with curves, all surfaces have an associated standard parameterization. In many cases the surfaces, as defined, are unbounded; it is assumed that they will be bounded either explicitly or implicitly. Explicit bounding is achieved with the bounded surface (here: plane); implicit bounding requires the association of additional topological information to define a face.