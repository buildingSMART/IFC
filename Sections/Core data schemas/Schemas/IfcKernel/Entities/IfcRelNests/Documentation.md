The nesting relationship _IfcRelNests_ is a special type of the general composition/decomposition (or whole/part) relationship _IfcRelDecomposes_. The nesting relationship can be applied to all subtypes of object, however it requires both the whole and the part to be of the same object type.

> <font size="-1">EXAMPLE: A nesting of costs is the composition
		of a complex cost from other costs. A nesting of work tasks is the composition
		of an overall work task from more specific work tasks. In all cases the whole
		has the same type as the parts.</font>

Decompositions imply a dependency, i.e. the definition of the whole depends on the definition of the parts and the parts depend on the existence of the whole. The behavior that is implied from the dependency has to be established inside the applications.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2.0.</font>
>
