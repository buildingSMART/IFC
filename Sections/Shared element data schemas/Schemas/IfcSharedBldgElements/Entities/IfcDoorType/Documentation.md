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

{ .use-head}
Operation type use definition

The _IfcDoorTypeOperationEnum_ defines the general layout of the door type and its symbolic presentation. Depending on the enumerator, the appropriate instances of _IfcDoorLiningProperties_ and _IfcDoorPanelProperties_ are attached in the list of _HasPropertySets_. The _IfcDoorTypeOperationEnum_ mainly determines the hinge side (left hung, or right hung), the operation (swinging, sliding, folding, etc.) and the number of panels.

> NOTE&nbsp; There are different definitions in various countries on what a left opening or left hung or left swing door is (same for right). Therefore the IFC definition may derivate from the local standard and may need to be mapped appropriately.

See geometry use definitions at _IfcDoorTypeOperationEnum_ for the correct usage of opening symbols for different operation types.

{ .use-head}
Material Use Definition

The material of the _IfcDoorType_ is defined by the _IfcMaterialConstituentSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

The following keywords for _IfcMaterialConstituentSet.MaterialConstituents[n].Name_ shall be used:

* 'Lining' - to indicate that the material constituent applies to to the door lining
* 'Framing' - to indicate that the material constituent applies to to the door framing, if not provided, the 'Lining' material information applied to frams as well
* 'Glazing' - to indicate that the material constituent applies to to the glazing as well

If the fall back single _IfcMaterial_ is referenced, it applies to the lining and framing of the door.

{ .use-head}
Geometry Use Definitions:

The _IfcDoorType_ may define the common shape of door occurrences. The common shape can be defined by

* applying shape parameters defined within the associated _IfcDoorLiningProperties_ and _IfcDoorPanelProperties_ applied to the 'Profile' geometric representation. It is only applicable if the _IfcDoorType_ has only occurrences of type _IfcDoorStandardCase_ (See geometric use definition of _IfcDoorStandardCase_ for further information).
* applying the _RepresentationMaps_ attribute to refer to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShapeRepresentation_'s having an _RepresentationIdentifier_ 'Box', 'Profile', 'FootPrint', or 'Body') 
>> NOTE&nbsp; The product shape representations are defined as _RepresentationMaps_ (attribute of the supertype _IfcTypeProduct_), which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[n]_ being an _IfcMappedItem_. See _IfcTypeProduct_ for further information. 
>> NOTE&nbsp; The values of attributes _RepresentationIdentifier_ and _RepresentationType_ of _IfcShapeRepresentation_ are restricted in the same way as those for _IfcDoor_ and _IfcDoorStandardCase_
