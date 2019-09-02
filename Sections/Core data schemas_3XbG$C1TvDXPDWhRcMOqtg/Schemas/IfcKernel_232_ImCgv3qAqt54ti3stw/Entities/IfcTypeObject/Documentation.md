The object type (_IfcTypeObject_) defines the specific information about a type. It refers to the specific level of the well recognized _generic - specific - occurrence_ modeling paradigm.

The object style is represented by a list of property set definitions, where the order in the list implies a decreasing generality. The list of property sets describes the available specific information about the object type. Thereby the object type is used to define the common properties of a certain type (or style) of an object that may be applied to multiple instances of the same type. The _IfcTypeObject_ gets assigned to the individual object instances (the occurrences) via the _IfcRelDefinesByType_ relationship.

Object types may be exchanged without being already assigned to objects. An object type may have an indication of the library (or catalogue) from which its definition originates. This association is handled by the inherited _HasAssociations_ relationship.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2x.</font>
>