**Definition
from IAI**: The _IfcRoot_ is the most abstract and root class for all IFC entity definitions that roots in the kernel or in subsequent layers of the IFC object model. It is therefore the common supertype all all IFC entities, beside those defined in an IFC resource schema. All entities that are subtypes of _IfcRoot_ can be used independently, whereas resource schema entities, that are not subtypes of _IfcRoot_, are not supposed to be independent entities.

The _IfcRoot_ assigns the globally unique ID, and the ownership and history information to the entity. In addition it may provide for a name and a description about the concepts.

> <font color="#0000ff" size="-1"> HISTORY New entity
in IFC Release 1.0 </font>