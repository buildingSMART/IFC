An _IfcFurnitureStandard_ is a standard for furniture allocation that can be assigned to persons within an organization.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x</font>

### Use Definitions
A furniture standard is assigned a set of classification notations (through the _IfcRelAssociatesClassification_ class within the _IfcKernel_ schema) that determine the types of furniture that fulfill the requirements of the standard. In order to use the IfcFurnitureStandard class, a classification of furniture items must have been established. This does not mean that each individual furniture item needs to have a classification notation although this is considered to be desirable.

A furniture standard is assigned to one or several persons or organizations (like a work group or department) through the _IfcRelAssignsToControl_ relationship via the _Controls_ inverse attribute.