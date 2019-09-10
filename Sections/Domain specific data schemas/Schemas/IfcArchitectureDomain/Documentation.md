The _IfcArchitectureDomain_ schema defines basic object concepts used in the architectural domain that have not been generalized and push lower in the model (e.g. shared with other domains or application types).

### Scope
Specific architectural elements that are not already covered by other schemas (most architectural elements are defined within the _IfcSharedBldgElements_ schema). Currently it includes:

* specific permeable covering properties for window and door openings
* space programs for design briefs, together with interaction requirements between spaces covered by space programs

### Definitions referenced from other schemas
**Resources**

Placement and geometry - defined by the supertype _IfcProduct_ and links the resource definitions of geometric contraints, representation, geometry, topology and geometric models.

Fundamental properties - Costs, classification, materials and documents: all of these concepts are related to most of the objects used by architects through the object supertypes defined at in the IFC core model. Those essential properties are connected by objectified relationships. See the fully attributed view of the entity definitions to find the objectified relationships.

**IfcKernel**

Single project reference - the _IfcProject_ is a single instance within an IFC file or database and links the spatial structure objects, the units and the representation context.

Actors - people and/or organizations involved in the project. Actors are important in the IFC model as they concepts such as ownership, responsibility, approval and workflow.

Assemblies -of elements. This concept is modeled using the objectified relationship _IfcRelAggregates_. Examples in architecture include stairs, ramps, curtain walls and roofs. The distinction from Nesting is that elements in an assembly can be of various types.

Controls - conceptual objects that determine or constrain other objects. IFC includes several examples of such controls (constraints, budgets, design program). These are related to the objects which they 'control' through the _IfcRelAssignsToControl_ objectified relationship. Examples that are of interest to architects include budgets, building code constraints, geometric alignment constraints and space programs (client brief information).

Groups - of objects, related for some group purpose. Object collections are related to a group object (which defines the purpose) through the _IfcRelAssignsToGroup_ objectified relationship.

Nesting - elements that contain other, like elements. This concept is modeled in IFC using the objectified relationship, _IfcRelNests_. This relationship requires that both, nested and nesting object are of the same object type.

Processes and resources - which process products (building elements), resulting in other products (assembly, refined or modified building elements, etc.). The most common examples of are construction processes.

Proxy objects - surrogates for types of objects that are not yet included in IFC. Proxies are included in IFC in the recognition that IFC will never fully elaborate all of the objects, concepts and processes in the AEC industry. This surrogate allows enables a basic representation of the 'foreign object type' so that the project model is a complete (if not totally accurate) representation. Architects will be most interested in product proxies. Surrogates for real world, physical objects. A shape representation and placement are included for such proxies. This allows architects to understand the shape, location and orientation of the real world object represented by the proxy.

Dynamically assigned properties - properties that are attached to objects and may be tailored by mutual agreements on the property names. This concept is handled through use of the objectified relationship _IfcRelDefinedByProperties_.

Type objects - allow the assignment of a type (or specific object) to all occurrencies of that type. This concept is handled through use of the objectified relationship _IfcRelDefinedByType_.

**IfcProductExtension**

Spatial structure objects - Site, building, building storey, space are used to contain architectural objects within a spatial structure.

Containment in spatial structure - elements that are contained in any level of the spatial project structure (site, building, building story, space). This concept is modeled using the objectified relationship _IfcRelContainedInSpatialStructure_.

Connections - between elements in a project. This concept is modeled in IFC using the objectified relationship _IfcRelConnectsElements_. Architects are interested many different types of connections because they must design construction details for them. Examples include wall to wall, wall to floor, wall to ceiling and column to beam connections. See _IfcRelConnectsElements_, its subtypes, the referenced _IfcConnectionGeometry_, its subtypes for more discussion on this subject.

Coverings - that cover other building elements. These objects have a special relationship, _IfcRelCoversBldgElements_, to other building elements which they 'cover'. Examples include floor and wall coverings, protective coverings (base molding, chair railing) and ceilings.

Grids - the design grid objects are provided through _IfcGrid_ and _IfcGridPlacement_. It is used to place objects relative to virtual grid intersections.

Space Boundaries - both physical and virtual elements which bound a space. Architects deal extensively with finishes in spaces and often specify such 'interior finishes' for the walls, floor(s) and ceilings that bound a space. IFC includes a special list of relationships from spaces to space boundaries. See _IfcSpace_ and _IfcRelSpaceBoundary_.

Zones - the_IfcZone_ object allows architects to compartmentize buildings in order to meet requirements of e. g., fire codes.

**IfcSharedBldgElements**

Walls, doors, windows, columns, beams, floors, roofs - all of these objects types, essential to architectural design are defined in the shared building elements schema because other disciplines also deal with them. Most of these allow specification of 'types' and association of more detailed properties associated with those types.

**IfcSharedBldgServiceElements**

Distribution systems (e.g., ducting, piping, sanitary, etc.), equipment, electrical appliances many types of these concepts are available in this release of IFC. The basic occurrence object types are accompanied by type objects defined in various building service and electrical specific domain schemas.

**IfcSharedFacilitiesElements**

Furniture - both standalone and systems furniture are available as type information for _IfcFurnishingElement_.

Occupant and Occupancy - architects deal with these concepts in the design and permit phases of projects. Facilities managers use them through the operations phase.