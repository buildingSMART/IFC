The element type _IfcWindowType_ defines commonly shared information for occurrences of windows. The set of shared information may include:

* common properties within shared property sets
* common material information
* common partitioning of panels
* common operation types of panels
* common shape representations

A window type defines the particular parameter of the lining and one (or several) panels through the _IfcWindowLiningProperties_ and the _IfcWindowPanelProperties_ as predefined property sets applicable to windows only.

It is used to define a window specification, or window style (the specific product information that is common to all occurrences of that window type). Window types may be exchanged without being already assigned to occurrences.

Occurrences of the _IfcWindowType_ within building models are represented by instances of _IfcWindow_.

> HISTORY&nbsp; New entity in IFC4. The entity _IfcWindowType_ replaces the previous definition _IfcWindowStyle_ (which is deprecated in IFC4).
