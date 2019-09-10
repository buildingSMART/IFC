An _IfcObject_ is the generalization of any semantically treated thing or process. Objects are things as they appear - i.e. occurrences.

> <font size="-1"> NOTE Examples of <i>IfcObject</i>
include physically tangible items, such as wall, beam or covering,
physically existing items, such as spaces, or conceptual items, such as
grids or virtual boundaries. It also stands for processes, such as work
tasks, for controls, such as cost items, for actors, such as persons
involved in the design process, etc. </font>

Objects can be named, using the inherited _Name_ attribute, which should be a user recognizable label for the object occurrence. Further explanations to the object can be given using the inherited _Description_ attribute. The _ObjectType_ attribute is used:

* to store the user defined value for all subtypes of _IfcObject_, where a _PredefinedType_ attribute is given, and its value is set to USERDEFINED.
* to provide a type information (could be seen as a very lightweight classifier) of the subtype of _IfcObject_, if no _PredefinedType_ attribute is given. This is often the case, if no comprehensive list of predefined types is available.

Objects are independent pieces of information that might contain or reference other pieces of information. There are four essential kind of relationships in which objects can be involved:

* **Assignment of other objects** - an assignment relationship that refers to other types of objects. See supertype _IfcObjectDefinition_ for more information.
* **Association to external resources** - an association relationship that refers to external sources of information.&nbsp;See supertype _IfcObjectDefinition_ for more information.
* **Aggregation of other objects** - an aggregation relationship that establishes a whole/part relation. See supertype _IfcObjectDefinition_ for more information.      
* **Refinement by type and properties** - a refinement relationship (_IfcRelDefines_) that uses a type definition or (partial) property set definition to define the properties of the object instance. It is a specific - occurrence relationship with implied dependencies (as the occurrence properties depend on the specific properties).

> <small><font color="#0000ff">HISTORY
New Entity in IFC Release 1.0 </font></small>
