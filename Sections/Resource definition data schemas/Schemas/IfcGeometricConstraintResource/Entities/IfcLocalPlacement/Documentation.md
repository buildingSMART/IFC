﻿An _IfcLocalPlacement_ defines the relative placement of a product in relation to the placement of another product or the absolute placement of a product within the geometric representation context of the project.

The _IfcLocalPlacement_ allows that an _IfcProduct_ can be placed by this _IfcLocalPlacement_ (through the attribute_ObjectPlacement_) within the local coordinate system of the object placement of another _IfcProduct_, which is referenced by the _PlacementRelTo_. Rules to prevent cyclic relative placements have to be introduced on the application level.

If the _PlacementRelTo_ is not given, then the _IfcProduct_ is placed absolutely within the world coordinate system.

The following conventions shall apply as default relative positions if the relative placement is used. The conventions are given for all five direct subtypes of _IfcProduct_, the _IfcSpatialStructureElement_, _IfcElement_, _IfcAnnotation_, _IfcGrid_, _IfcPort_. More detailed placement information is given at the level of subtypes of those five types mentioned.

* For the subtypes of _IfcSpatialStructureElement_ the following conventions apply 
    * _IfcSite_ shall be placed absolutely within the world coordinate system established by the geometric representation context of the _IfcProject_ 
    * _IfcFacility_ shall be placed relative to the local placement of _IfcSite_ 
    * _IfcFacilityPart_ shall be placed relative to the local placement of _IfcFacility_ 
* For _IfcGrid_ and _IfcAnnotation_ the convention applies that it shall be placed relative 
    *  to the local placement of its container, either _IfcSite_, _IfcBuilding_, or _IfcBuildingStorey_ 
        * it should be the same container element that is referenced by the _IfcRelContainedInSpatialStructure_ containment relationship, 
*  For _IfcAlignment_ placed relative to the local placement of its container _IfcSite_ when not placed absolutely within the world coordinate system. 
* For _IfcPort_ the convention applies that it shall be placed relative 
    *  to the local placement of the _IfcElement_ it belongs to 
        * it should be the same element that is referenced by the _IfcRelConnectsPortToElement_ connection relationship, 
*  For _IfcElement_ the convention applies that it shall be placed relative: 
    *  to the local placement of its container, either _IfcSite_, _IfcFacility_, or _IfcFacilityPart_ 
        * it should be the same container element that is referenced by the _IfcRelContainedInSpatialStructure_ containment relationship, 
    * to the local placement of the _IfcElement_ to which it is tied by an element composition relationship 
        * for features that are located relative to the main component (such as openings), as expressed by _IfcRelVoidsElement_ and _IfcRelProjectsElement_;
        * for elements that fill an opening (such as doors or windows), as expressed by _IfcRelFillsElement_;
        * for coverings that cover the element, as expressed by _IfcRelCoversBldgElements_;
        * for sub components that are aggregated to the main component, as expressed by _IfcRelAggregates_ and _IfcRelNests_. 

> HISTORY&nbsp; New entity in IFC1.0.
