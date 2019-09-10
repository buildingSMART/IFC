Generalization of all furniture related objects. Furnishing objects are characterized as being

* pre-manufactured and assembled on-site, or 
* manufactured on-site (built-in) 

Thus furnishing elements can either be movable, or not (as the built-ins).

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
        Release 2x.</font>
> 


****Geometry Use Definitions****:

The geometric representation of _IfcFurnishingElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcFurnishingElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ , which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Any _IfcFurnishingElement_ can be represented by one or several geometric representations. This includes the general representation types 'BoundingBox', 'GeometricCurveSet', 'SurfaceModel', 'Brep', and 'MappedRepresentation' being defined here.

**Bounding Box Representation**

Any _IfcFurnishingElement_ may be represented as a bounding box, which shows the maximum extend of the body within the coordinated system established by the _IfcLocalPlacement_. The bounding box representation is the simplest geometric representation available. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Box' 
*  _RepresentationType_ : 'BoundingBox' 

**Foot Print Representation**

The foot print representation of _IfcFurnishingElement_ is given by either a single or multiple 2D points and curves. The representation identifier and type of this geometric representation are:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint' 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' 

**SurfaceModel Representation**

Any _IfcFurnishingElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple surface models, based on either shell or face based models. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape. The representation identifier and type of this geometric representation are:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body' 
*  _IfcShapeRepresentation.RepresentationType_ = 'SurfaceModel' 

**Brep Representation**

Any _IfcFurnishingElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation elements (which are restricted to faceted Brep with or without voids). The Brep representation allows for the representation of complex element shape. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape. The representation identifier and type of this geometric representation are:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body' 
*  _IfcShapeRepresentation.RepresentationType_ = 'Brep' 

**MappedRepresentation**

The _IfcMappedItem_ should always be used in appropriate cases as it allows for reusing the geometry definition of the furnishing type for all occurrences of the same type. The representation identifier and type of this geometric representation are:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint', or 'Body' (depending of the representation map) 
*  _IfcShapeRepresentation.RepresentationType_ = 'MappedRepresentation'
