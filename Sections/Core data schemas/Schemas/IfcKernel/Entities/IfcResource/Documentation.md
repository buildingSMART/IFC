The _IfcResource_ contains the information needed to represent the costs, schedule, and other impacts from the use of a thing in a process. It is not intended to use _IfcResource_ to model the general properties of the things themselves, while an optional linkage from _IfcResource_ to the things to be used can be specified (i.e. the relationship from subtypes of _IfcResource_ to _IfcProduct_ through the _IfcRelAssignsToResource_ relationship).

There are two basic intended use of _IfcResource_. First, if the attributes of the thing are not needed for the purpose of the use of _IfcResource_, or the types of things are not explicitly modeled in IFC yet, then the linkage between the resource and the thing doesn&#146;t have to be instantiated in the system. That is, the attributes of _IfcResource_ (or its subtypes) alone are sufficient to represent the use of the thing as a resource for the purpose of the project.

> <font size="-1">EXAMPLE: construction equipment such as earth-moving
		  vehicles or tools are not currently modeled within the IFC. For the purpose of
		  estimating and scheduling, these can be represented using subtypes of
		  IfcResource alone.</font>
>

Second, if the attributes of the thing are needed for the use of _IfcResource_ objects, and they are modeled explicitly as objects (e.g. classes or properties), then the _IfcResource_ instances can be linked to the instances of the type of the things being referenced. Things that might be used as resources and that are already modeled in the IFC include physical products, people and organizations, and materials. The relationship object _IfcRelAssignsToResource_ is provided for this approach.

The inherited attribute _ObjectType_ is used as a textual code that identifies the resource type.

> <font color="#0033FF" size="-1">HISTORY New entity in IFC
		Release 1.0</font>

> <font size="-1" color="#FF0000">IFC2x PLATFORM CHANGE: The
		attributes BaseUnit and ResourceConsumption have been removed from the abstract
		entity, they are reintroduced at a lower level in the
		hierarchy.</font>