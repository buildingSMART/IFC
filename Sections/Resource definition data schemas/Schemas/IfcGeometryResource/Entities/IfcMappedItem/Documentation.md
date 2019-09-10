**Definition
from ISO/CD 10303-43:1992**: A mapped item is the use of an existing representation (the mapping source - mapped representation) as a representation item in a second representation.

> <font size="-1">NOTE: A mapped item is a subtype of
representation item. It enables a representation to be used as a
representation item in one or more other representations. The mapped
item allows for the definition of a representation using other
representations. </font>
> 


**Definition
from IAI**: The _IfcMappedItem_ is the inserted instance of a source definition (to be compared with a block / shared cell / macro definition). The instance is inserted by applying a Cartesian transformation operator as the _MappingTarget_.

> <font size="-1">EXAMPLE&nbsp; An <i>IfcMappedItem</i>
can reuse other
mapped items (ako nested blocks), doing so the <i>IfcRepresentationMap</i>
is based on an <i>IfcShapeRepresentation</i>
including one or more <i>IfcMappedItem</i>'s.<br>
  </font>
> 
> <font color="#0000ff" size="-1">NOTE &nbsp;
Corresponding STEP entity: mapped_item. Please refer to ISO/IS
10303-43:1994, for the final definition of the formal standard. The
definition of mapping_target (<i>MappingTarget</i>)
has been restricted to be of the type cartesian_transformation_operator
(<i>IfcCartesianTransformationOperator</i>).</font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC Release 2x. </font>
> 


**Informal
Propositions**

1. A mapped item shall not be self-defining by participating in the definition of the representation being mapped.
2. The dimensionality of the mapping source and the mapping target has to be the same, if the mapping source is a geometric representation item.
