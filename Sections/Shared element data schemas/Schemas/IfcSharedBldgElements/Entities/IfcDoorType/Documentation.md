﻿The element type _IfcDoorType_ defines commonly shared information for occurrences of doors. The set of shared information may include:

* common properties within shared property sets
* common material information
* common operation type definitions
* common shape representations

A door type defines the particular parameter of the lining and one (or several) panels through the _IfcDoorLiningProperties_ and the _IfcDoorPanelProperties_ as predefined property sets applicable to doors only.

It is used to define a door specification, or door style (i.e. the specific product information that is common to all occurrences of that door type). Door types may be exchanged without being already assigned to occurrences.

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which gets assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

Occurrences of the _IfcDoorType_ within building models are represented by instances of _IfcDoor_.

> HISTORY&nbsp; New entity in IFC4. The entity _IfcDoorType_ replaces the previous definition _IfcDoorStyle_ (which is deprecated in IFC4).
