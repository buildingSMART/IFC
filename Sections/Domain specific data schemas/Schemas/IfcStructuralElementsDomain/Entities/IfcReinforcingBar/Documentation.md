A steel bar, usually with manufactured deformations in the surface, used in concrete and masonry construction to provide additional strength.

> <font color="#0000ff" size="-1">
HISTORY New entity in IFC
Release 2x2 </font>

****Property Set Use Definition****:

The property sets relating to the _IfcReinforcingBar_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcReinforcingBar_ are part of this IFC release:

* [Pset_ReinforcingBarBendingsBECCommon](../../psd/IfcStructuralElementsDomain/Pset_ReinforcingBarBendingsBECCommon.xml){ target="SOURCE"}: common property set for all _IfcReinforcingBar_ occurrences for bending information according to the Finnish BEC-standard. 
* [Pset_ReinforcingBarBendingsBS8666Common](../../psd/IfcStructuralElementsDomain/Pset_ReinforcingBarBendingsBS8666Common.xml){ target="SOURCE"}: common property set for all _IfcReinforcingBar_ occurrences for bending information according to the BS8666 standard. 
* [Pset_ReinforcingBarBendingsDIN135610Common](../../psd/IfcStructuralElementsDomain/Pset_ReinforcingBarBendingsDIN135610Common.xml){ target="SOURCE"}: common property set for all _IfcReinforcingBar_ occurrences for bending information according to the DIN 1356-10 standard. 
* [Pset_ReinforcingBarBendingsISOCD3766Common](../../psd/IfcStructuralElementsDomain/Pset_ReinforcingBarBendingsISOCD3766Common.xml){ target="SOURCE"}: common property set for all _IfcReinforcingBar_ occurrences for bending information according to the ISO CD 3766 standard. 

**Geometry Use Definitions:**

The geometric representation of _IfcReinforcingBar_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The use of local placement is defined at the supertype _IfcBuildingElementComponent_.

**Standard Geometric Representation using Swept Solid
Representation**  
The standard geometric representation of _IfcReinforcingBar_ is defined using the swept solid representation. The _RepresentationType_ attribute of _IfcShapeRepresentation_ should have the value 'SweptSolid'. The solid is formed from a cross section approximated as a circular disk swept along any arbitrary curve. Given this, the following constraints apply to the standard representation:

* **Solid:** _IfcSweptDiskSolid_ introduced in IFC Release 2x2 shall be supported. 
* **Profile:** The circular disk cross section approximation is defined by the _Radius_ attribute of _IfcSweptDiskSolid_. 
* **Extrusion:** The extrusion along any arbitrary curve is defined by the _Directrix_ attribute of _IfcSweptDiskSolid_. 

**Simplified Geometric Representation**  
Simplified geometric representations may be used based on local agreements.