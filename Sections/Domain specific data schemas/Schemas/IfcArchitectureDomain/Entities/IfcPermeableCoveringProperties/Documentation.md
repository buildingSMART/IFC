﻿This entity is a description of a panel within a door or window (as fillers for opening) which allows for air flow. It is given by its properties (_IfcPermeableCoveringProperties_). A permeable covering is a casement, such as a component, fixed or opening, consisting essentially of a frame and the infilling. The infilling is normally a grill, a louver or a screen. The way of operation is defined in the operation type.

The _IfcPermeableCoveringProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcWindowStyle_ or the _IfcDoorStyle_. More information about the permeable covering can be included in the same list of the window or door style using the _IfcPropertySet_ for dynamic extensions. This particularly applies for additional properties for the various operation types

The _IfcPermeableCoveringProperties_ does not hold a geometric representation. However it defines parameters which can be used to create the shape of the _IfcWindowStyle_ (which is inserted by the _IfcWindow_ into the spatial context of the project), or of the _IfcDoorStyle_ (which is inserted by the _IfcDoor_).

The parameters at the _IfcPermeableCoveringProperties_ define a standard permeable covering. The outer boundary of the panel is determined by the occurrence parameter assigned to the _IfcWindow_ or _IfcDoor_. It has to take the lining parameter into account as well. The position of the permeable covering within the overall window or door is determined by the _PanelPosition_ attribute.

Figure 1 illustrates the panel applied to the position within the lining, as defined by the panel position attribute. The following parameters apply to that panel: _FrameDepth_, _FrameThickness_.

!["covering"](../../../../../../figures/ifcpermeablecoveringproperties.gif "Figure 1 &mdash; Permeable covering properties")

> HISTORY&nbsp; New entity in IFC2.0, it had been renamed from _IfcPermeableCovering_ in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Supertype changed to new _IfcPreDefinedPropertySet_.
