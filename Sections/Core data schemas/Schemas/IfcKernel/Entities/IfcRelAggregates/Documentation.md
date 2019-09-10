The aggregation relationship _IfcRelAggregates_ is a special type of the general composition/decomposition (or whole/part) relationship _IfcRelDecomposes_. The aggregation relationship can be applied to all subtypes of object.

Some further specializations of decomposition may imply additional constraints and meanings, such as the requirement of aggregates to represent physical containment. In cases of physical containment the representation (within the same representation context) of the whole can be taken from the sum of the representations of the parts.

> <font size="-1">EXAMPLE: A roof is the aggregation of the roof
		elements, such as roof slabs, rafters, purlins, etc. Within the same
		representation context, e.g. the detailed geometric representation, the shape
		representation of the roof is given by the shape representation of its
		parts</font>

Decompositions imply a dependency, i.e. the definition of the whole depends on the definition of the parts and the parts depend on the existence of the whole. The behavior that is implied from the dependency has to be established inside the applications.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2x.</font>
>
