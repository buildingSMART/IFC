This objectified relationship (_IfcRelAssignsToActor_) handles the assignment of objects (subtypes of _IfcObject_) to an actor (subtypes of _IfcActor_).

The _IfcRelAssignsToActor_ objectified relationship defines a relationship between an _IfcActor_ and one or many objects. An particular role of the actor played in that relationship can be associated. If specified, it takes priority over the role that may be directly assigned to the person or organization.

> **Example**: An occupant (as an actor) may rent (as a special association type) a flat (as a collection of spaces or a zone). This would be an application of this generic relationship.

Reference to the objects (or single object) on which the actor acts upon in a certain role (if given) is specified in the inherited _RelatedObjects_ attribute.

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC Release 2.0.
		  Has been renamed from IfcRelActsUpon in IFC Release 2x.</font>
>
