The schema _IfcKernel_ defines the most abstract part within the IFC architecture. It captures general constructs, that are basically founded by their different semantic meaning in common understanding of an object model, like object, property and relationship. Those are then specialized into non-AEC/FM specific constructs, like product, process, control and resource, which form the main entry points for the next level, the Core Extension layer.

The _IfcKernel_ utilizes the translation of the IFC Meta model into IFC object model specification. It handles the basic functionality, such as relative location of products in space, sequence of processes in time, or general purpose grouping and nesting mechanism. It also lays the foundation of extensibility of IFC model by providing:

* proxy definitions
*  type object definitions 
* property set definitions. 

### Concept of a root
Each entity defined in the core, interoperability or domain layer of the IFC model inherits (over some intermediate steps) from the _IfcRoot_ entity. It provides for the fundamental concepts of:

*  identification - assigning a globally unique identifier (the GUID)
* ownership and change information
* optional label attribution 

There are three fundamental entity types in the IFC model, which are all derived from _IfcRoot_. They form the 1^st^ level of specialization within the IFC class hierarchy.

* **objects** (_IfcObject_) - are the generalization of any semantically treated thing (or item) within the IFC model.
* **relations** (_IfcRelationship_) - are the generalization of all relationships among things (or items) that are treaded as objectified relationships in the IFC model
* **properties** (_IfcPropertyDefinition_) - are the generalization of all characteristics (either types or partial type, i.e. property sets) that may be assigned to objects 

### Concept of an object
An object is the abstract supertype, _IfcObject_, and stands for all physically tangible items, such as wall, beam or covering, physically existing items, such as spaces, or conceptual items, such as grids or virtual boundaries. It also stands for processes, such as work tasks, for controls, such as cost items, for resources, such as labor resource, or for actors, such as persons involved in the design process, etc.

An object gets its context information from the relationships in which it is involved. The property information and, if available, the information about the underlying specific object type. An object may have an informal type descriptor assigned, which denotes a particular type to further specifies the object.

### Concept of a relationship
A concept of relationships is the objectified relationship, _IfcRelationship_. The objectified relationship is the preferred way to handle relationships among objects. This allows to keep relationship specific properties directly at the relationship object and to uncouple the relationship semantics from the object attributes.

The introduction of the objectified relationships also allows the development of a separate subtype tree for relationship semantics.

### Concept of a property definition
The property definition, _IfcPropertyDefinition_, is the generalization of all characteristics of objects. Shared among multiple object instances, it reflects the specific information of an object type, but it may also represent the occurrence information of the actual object in the project context, if it is assigned only to a single object instance.

The property definition gets applied to the objects using the concept of relationships.

### Object entity subtype tree
There are seven fundamental entity types in the IFC model, which are all derived from _IfcObject_. They form the 2^nd^ level of specialization within the IFC class hierarchy under the object branch.

*  **products** - are physical object (manufactured, supplied or created) for incorporation into a project. They may be physically existing or tangible. Products may be defined by shape representations and have a location in the coordinate space.
*  **processes** - are actions taking place in a project with the intent of, e.g., acquiring, constructing, or maintaining objects. Processes are placed in sequence in time.
*  **controls** - are concepts that control or constrain other objects. Controls can be seen as guide, specification, regulation, constraint or other requirement applied to an object that has to be fulfilled.
*  **resources** - are concepts that describe the use of an object mainly within a process.
*  **actors** - are human agents that are involved in a project during its full life cycle.
*  **project** - is the undertaking of some engineering activities leading towards a product.
*  **group** - is an arbitrary collection of objects..

### Relationship entity subtype tree
There are five fundamental relationship types in the IFC model, which are all derived from _IfcRelationship_. They form the 2^nd^ level of specialization within the IFC class hierarchy under the relationship branch.

A relationship may have an informal purpose descriptor assigned, which denotes a particular purpose of applying this relationship.

*  **assignment** - is a generalization of "link" relationships among instances of objects and its various subtypes. A link denotes the specific association through which one object (the client) applies the services of other objects (the suppliers), or through which one object may navigate to other objects.
*  **association** - refers to external sources of information (most notably a classification, library or document) and associates it to objects or property definitions.
*  **decomposition** - defines the general concept of elements being composed or decomposed. The decomposition relationship denotes a whole/part hierarchy with the ability to navigate from the whole (the composition) to the parts and vice versa.
*  **definition** - uses a type definition or property set definition (seen as partial type information) to define the properties of the object instance. It is a specific - occurrence relationship
*  **connectivity** - handles the connectivity of objects.

### Property definition entity subtype tree
There are two fundamental concepts of property definition types in the IFC model, which are all derived from _IfcPropertyDefinition_. They form the 2^nd^ level of specialization within the IFC class hierarchy under the property definition branch.

* **type object** - defines the specific information about a type. It refers to the specific level of the well recognized _generic - specific - occurrence_ modeling paradigm.
* **property set definition** - defines shareable and extensible property sets attachable to occurrences of objects. The property set is regarded as a partial type information as it establishes a subset of common shared property information among occurrence objects. 

> <font size="-1" color="#0000FF">HISTORY This schema is new in
		IFC Release 1.5 </font>