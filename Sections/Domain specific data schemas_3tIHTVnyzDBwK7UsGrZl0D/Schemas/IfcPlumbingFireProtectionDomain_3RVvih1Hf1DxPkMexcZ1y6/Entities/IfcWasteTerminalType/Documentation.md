The flow terminal type **IfcWasteTerminalType** defines commonly shared information for occurrences of waste terminals. The set of shared information may include:

* common properties with shared property sets
* common representations
* common materials
* common composition of elements
* common ports

It is used to define a waste terminal type specification indicating the specific product information that is common to all occurrences of that product type. The **IfcWasteTerminalType** may be declared within _IfcProject_ or _IfcProjectLibrary_ using _IfcRelDeclares_ and may be exchanged with or without occurrences of the type. Occurrences of **IfcWasteTerminalType** are represented by instances of _IfcWasteTerminal_. Refer to the documentation at _IfcWasteTerminal_ for supported property sets, materials, composition, and ports.