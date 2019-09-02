An _IfcEquipmentStandard_ is a standard for equipment allocation that can be assigned to persons within an organization.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x</font>

### Use Definitions
An _IfcEquipmentStandard_ is assigned a set of classification notations (through the _IfcRelAssociatesClassification_ class within the _IfcKernel_ schema) that determine the types of equipment that fulfill the requirements of the standard. In order to use the equipment standard class, a classification of equipment items must have been established. This does not mean that each individual equipment item needs to have a classification notation although this is considered to be desirable. Examples of equipment items that might fall within an equipment standard include number and type PC's and connections, task lighting, pictures etc.

An equipment standard is assigned to one or several persons or organizations (like a work group or department) through the _IfcRelAssignsToControl_ relationship via the _Controls_ inverse attribute.