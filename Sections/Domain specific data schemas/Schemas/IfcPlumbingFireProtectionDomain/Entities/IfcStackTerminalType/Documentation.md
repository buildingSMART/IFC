The _IfcStackTerminalType_ defines a particular type of _IfcFlowTerminal_ placed at the top of a ventilating stack (to prevent ingress by birds, rainwater etc.) or rainwater pipe (to act as a collector or hopper for discharge from guttering).

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcStackTerminalType_ identifies a particular type of _IfcFlowTerminal_ that is placed at the top of a vertical pipe in a waste/drainage/rainwater system to fulfill a particular purpose. The purpose is by default in the context of the stack subsystem in which the terminal participates. The particular type of the stack terminal is defined by the set value of the stack terminal type enumeration.

An _IfcStackTerminalType_ may be included into the spatial context of the building model through an (or multiple) instances of _IfcFlowTerminal_.

****Property Set Use Definition****:

Note that there are no predefined property sets assigned to this type at present.

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.