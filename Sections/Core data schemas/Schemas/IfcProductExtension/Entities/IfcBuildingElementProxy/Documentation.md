The _IfcBuildingElementProxy_ is a proxy definition that provides the same functionality as an _IfcBuildingElement_, but without having a defined meaning of the special type of building element, it represents.

> <small>NOTE1 The <i>IfcBuildingElementProxy</i> should be
        used to exchange special types of building elements for
        which the current IFC Release does not yet provide a
        semantic definition.</small>
> 
> <small>NOTE2 The <i>IfcBuildingElementProxy</i> can also
        be used to represent building elements for which the
        participating applications can not provide additional
        semantic classification.</small>
> 


> <font color="#0000FF"><small>HISTORY New entity in IFC
        Release 2x.</small></font>
> 


****Type Use Definition****

The _IfcBuildingElementProxy_ defines the occurrence of any building element, common information about the types (or styles) is handled by _IfcBuildingElementProxyType_.

The _IfcBuildingElementProxyType_ (if present) may establish the common type name, usage (or predefined) type, common material, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcBuildingElementProxyType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

> <small>NOTE The <i>IfcBuildingElementProxyType</i> can be
        used to share common information among many occurrences
        of the same proxy without establishing a particular
        semantic meaning of the type.</small>
> 


If no _IfcBuildingElementProxyType_ is attached (i.e. if only occurrence information is given) the predefined type may be given by using the _ObjectType_ attribute.

****Property Set Use Definition****:

The property sets relating to the _IfcBuildingElementProxy_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcBuildingElementProxy/i> are part of this IFC release:_

*  [Pset_BuildingElementProxyCommon](../../psd/IfcProductExtension/Pset_BuildingElementProxyCommon.xml){ target="SOURCE"}: common property set for all occurrences of building element proxies. 

****Geometry Use Definitions****

The geometric representation of any _IfcBuildingElementProxy_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations. The representation types defined at the supertype _IfcBuildingElement_ also apply.

**Local Placement**

The local placement for any _IfcBuildingElementProxy_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations. The local placement can be given relatively.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

****Geometric Representation****

Currently, the use of the representation types 'BoundingBox', 'GeometricSet', 'GeometricCurveSet', 'SweptSolid', 'SurfaceModel', 'Brep', and 'MappedRepresentation' are allowed. The geometry use definitions for 'BoundingBox', 'SurfaceModel', 'Brep', and 'MappedRepresentation' are explained at the supertype _IfcBuildingElement_.

**GeometricCurveSet Representation**

Any building element proxy may be represented by a geometric curve set, given by a collection of 2D points and curves. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_: 'FootPrint' 
*  _RepresentationType_: 'GeometricCurveSet' 

**GeometricSet Representation**

Any building element proxy may be represented by a geometric set, given by a collection of 2D and 3D points, curves, and surfaces. It represents the body of the proxy object, when no topological structure is available. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_: 'Body' 
*  _RepresentationType_: 'GeometricSet' 

**Swept Solid Representation**

Any building element proxy may be represented by swept solid geometry (either by extrusion or by revolution). The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_: 'Body' 
*  _RepresentationType_: 'SweptSolid' 

No further restrictions (e.g., for the profile or extrusion direction) are defined at this level. A single or multiple swept area solid(s) can be the _Items_ of the _IfcShapeRepresentation_.
