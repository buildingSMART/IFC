**Definition
from IAI**: An _IfcObjectDefinition_ is the generalization of any semantically treated thing or process, either being a type or an occurrences. Object defintions can be named, using the inherited _Name_ attribute, which should be a user recognizable label for the object occurrence. Further explanations to the object can be given using the inherited _Description_ attribute.&nbsp;

Objects are independent pieces of information that might contain or reference other pieces of information. There are three essential kinds of relationships in which object definitions (by their instantiable subtypes) can be involved:

* **Assignment of other objects** - an assignment relationship (_IfcRelAssigns_) that refers to other types of objects and creates a bi-directional association. The semantic of the assignment is established at the level of the subtypes of the general _IfcRelAssigns_ relationship. There is no dependency implied a priori by the assignment.
* **Association to external resources** - an association relationship (_IfcRelAssociates_) that refers to external sources of information (most notably a classification or document) and creates a uni-directional association. There is no dependency implied by the association.
* **Aggregation of other objects** - an aggregation relationship (_IfcRelDecomposes_) that establishes a whole/part relation and creates a bi-directional relation. There is an implied dependency established.

> <small> <font color="#0000ff">HISTORY&nbsp;
New abstract entity in Release IFC2x Edition 3. </font><br>
  <font color="#ff0000">IFC2x Edition 3
CHANGE&nbsp; The
abstract entity <i>IfcObjectDefinition&nbsp;</i>has
been added. Upward compatibility for file
based exchange is guaranteed.</font> </small>
