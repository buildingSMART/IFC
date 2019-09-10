The element type _IfcWindowType_ defines commonly shared information for occurrences of windows. The set of shared information may include:

* common properties within shared property sets
* common material information
* common partitioning of panels
* common operation types of panels
* common shape representations

A window type defines the particular parameter of the lining and one (or several) panels through the _IfcWindowLiningProperties_ and the _IfcWindowPanelProperties_ as predefined property sets applicable to windows only.

It is used to define a window specification, or window style (the specific product information that is common to all occurrences of that window type). Window types may be exchanged without being already assigned to occurrences.

Occurrences of the _IfcWindowType_ within building models are represented by instances of _IfcWindow_ or _IfcWindowStandardCase_.

> HISTORY&nbsp; New entity in IFC4. The entity _IfcWindowType_ replaces the previous definition _IfcWindowStyle_ (which is deprecated in IFC4).

{ .use-head}
Geometry Use Definitions:

The _IfcWindowType_ may define the common shape of window occurrences. The common shape can be defined by

* applying shape parameters defined within the associated _IfcWindowLiningProperties_ and _IfcWindowPanelProperties_ applied to the 'Profile' geometric representation. It is only applicable if the _IfcWindowType_ has only occurrences of type _IfcWindowStandardCase_ (See geometric use definition of _IfcWindowStandardCase_ for further information).
* applying the _RepresentationMaps_ attribute to refer to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShapeRepresentation_'s having an _RepresentationIdentifier_ 'Box', 'Profile', 'FootPrint', or 'Body') 
>> NOTE&nbsp; The product shape representations are defined as _RepresentationMaps_ (attribute of the supertype _IfcTypeProduct_), which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[n]_ being an _IfcMappedItem_. See _IfcTypeProduct_ for further information. 
>> NOTE&nbsp; The values of attributes _RepresentationIdentifier_ and _RepresentationType_ of _IfcShapeRepresentation_ are restricted in the same way as those for _IfcWindow_ and _IfcWindowStandardCase_
