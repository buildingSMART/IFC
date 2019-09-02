An _IfcOrderAction_ is the point at which requests for work are received and processed within an organization.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC 2x2</font>

### Use Definitions
The _IfcOrderAction_ represents tasks that might be carried out by a Helpdesk acting the role of interface for the organization between the facility user and the functional requirement of fulfilling their needs. The actual task represented by the _IfcOrderAction_ class is turning a request into an order and initiating the action that will enable the order to be completed.

_IfcRelAssignsToControl_ is used to relate one or more instances of _IfcOrderAction_ to an _IfcProjectOrder_ or one of its subtypes including maintenance work order.