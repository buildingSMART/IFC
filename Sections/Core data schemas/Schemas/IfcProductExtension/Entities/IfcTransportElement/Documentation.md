Generalization of all transport related objects that move people, animals or goods within a building or building complex. The _IfcTransportElement_ defines the occurrence of a covering type, that (if given) is expressed by the _IfcTransportElementType_.

> <font size="-1">EXAMPLE: Transportation elements include
      elevator (lift), escalator, moving walkway, etc.</font>

> <font color="#FF0000" size="-1">IFC2x PLATFORM CHANGE: The
      attribute <i>OperationType</i> is now optional and should
      only be inserted when there is no type information, given
      by <i>IfcTransportElementType</i>, is assigned to the
      <i>IfcTransportElement</i> occurrence by
      <i>IfcRelDefinesByType</i>.</font>

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
        Release 2x.</font>
> 


****Property Set Use Definition****:

The property sets relating to the _IfcTransportElement_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcTransportElement_ are part of this IFC release:

*  [Pset_TransportElementCommon](../../psd/IfcProductExtension/Pset_TransportElementCommon.xml){ target="SOURCE"}: common property set for all transport element occurrences 
*  [Pset_TransportElementElevator](../../psd/IfcProductExtension/Pset_TransportElementElevator.xml){ target="SOURCE"}: specific property set for all occurrences of transport elements with the _PredefinedType_: ELEVATOR 

****Geometry Use Definitions****:

The geometric representation of _IfcTransportElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcTransportElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ , which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**SurfaceModel Representation**

Any _IfcTransportElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple surface models, based on either shell or face based models. Then the following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SurfaceModel' 

**Brep Representation**

Any _IfcTransportElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation elements (which are restricted to faceted Brep with or without voids). Then the following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'Brep' 

**MappedRepresentation**

The new mapped item, _IfcMappedItem_, should be used if appropriate as it allows for reusing the geometry definition of the property element type at occurrences of the same equipment type. Then the following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'MappedRepresentation'