The decomposition relationship, _IfcRelDecomposes_, defines the general concept of elements being composed or decomposed. The decomposition relationship denotes a whole/part hierarchy with the ability to navigate from the whole (the composition) to the parts and vice versa.

Decompositions may be constraint by requiring both, the whole and its parts, to be of the same type - thus establishing a nesting relationship. Or they may require some form of physical containment, thus establishing special types of aggregation relationships.

> <font size="-1"> NOTE: There are two special names for
		decomposition, which are linguistically distinguished, nesting and aggregation.
		The subtypes of <i>IfcRelDecomposes</i> will introduce either the nesting or
		aggregation convention (see <i>IfcRelNests</i> and
		<i>IfcRelAggregates</i>).</font>

> <font size="-1"> EXAMPLE: A cost element is a nest of other
		cost elements. Or a structural frame is an aggregation of beams and columns.
		Both are applications of decomposition relationship.</font>

Decompositions imply a dependency, i.e. the definition of the whole depends on the definition of the parts and the parts depend on the existence of the whole. The decomposition relationship can be applied in a recursive manner, i.e. a decomposed element can be part in another decomposition. Cyclic references have to be prevented at application level.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 1.5,
		  it is a generalization of the IFC2.0 entity IfcRelNests.</font>
>