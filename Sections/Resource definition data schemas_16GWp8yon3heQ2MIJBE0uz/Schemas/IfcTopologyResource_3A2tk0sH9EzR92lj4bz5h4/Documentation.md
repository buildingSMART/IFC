The schema _IfcTopologyResource_ defines the resources used for topological representations. The primary application of this resource is its use in the Boundary representation of the shape or geometric form of a product model.

> <font color="#0000FF">NOTE: The definitions of this resource of
		the IFC model have been taken from the Integrated Resource, part 42 "Integrated
		generic resources: Geometric and topological representations" of the ISO
		standard 10303: "Industrial automation systems and integration - Product data
		representation and exchange". The IfcTopologyResource refers to the clause 5,
		"Topology" of the standard. The reference is ISO/IS 10303-42:1994, pp. 122. The
		improved definitions of the second edition, ISO/DIS 10303-42:1999 have been
		used, when applicable.</font>

The definitions taken from ISO/IS 10303-42:1994 have undergone an adaptation process, characterized by:

* adaptation of the IFC naming convention (inner majuscules and Ifc prefix)
* adaptation of the STEP entities, where multiple inheritance or non-exclusive inheritance (i.e. AND or ANDOR subtype constraints) are used
* selection of a subset of the IR, using subtype and select pruning
* omission of the name attribute at the representation item

The topological representation of the shape is defined following the adaptation of the **ISO/CD 10303-42:1992**, _Industrial Automation Systems
		and Integration: Product Data Representation and Exchange - Part 42: Integrated
		Generic Resources. Geometric and Topological Representation_. The type, class, and function semantic definition sections follow the adapted wording of the working draft, which is clearly indicated and quoted at each reference. The definitions on geometric and topological representation (when taken from ISO/CD 10303-42:1992) are explicitly excluded from the copyright of the International Alliance of Interoperability.

> <font color="#0000FF">For more information on the definitions
		as defined in the formal ISO standard please refer to: ISO/IS 10303-42:1994,
		Industrial Automation Systems and Integration: Product Data Representation and
		Exchange - Part 42: Integrated Generic Resources. Geometric and Topological
		Representation. The formal standard can be obtained through the local
		publishers of standards in each individual country.</font>

The following are within the scope of the topology schema:

* definition of the fundamental topological entities vertex, edge, and face, each with a specialized subtype to enable it to be associated with the geometry of a point, curve, or surface, respectively; 
* collections of the basic entities to form topological structures of path, loop and shell and constraints to ensure the integrity of these structures;
* orientation of topological entities.