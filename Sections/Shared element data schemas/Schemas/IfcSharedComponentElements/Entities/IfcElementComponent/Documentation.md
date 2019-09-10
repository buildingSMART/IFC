An element component is a representation for minor items included in, added to or connecting to or between elements, which usually are not of interest from the overall building structure viewpoint. However, these small parts may have vital and load carrying functions within the construction. These items do not provide any actual space boundaries. Typical examples of _IfcElementComponent_s include different kinds of fasteners and various accessories.

> <font color="#0000FF" size="-1">
   HISTORY New entity in IFC Release 2x2
</font>

**Geometry Use Definitions:**

The geometric representation of _IfcElementComponent_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The local placement for _IfcElementComponent_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcElement_ or _IfcElementAssembly_, which is used in the _Decomposes_ inverse attribute, i.e. the local placement is defined relative to the local placement of the element or element assembly in which the component is contained. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**Surface Model Representation**  
Any _IfcElementComponent_ (if no further constraints are defined at the level of its subtypes) may be represented as a single or multiple surface models, based on either shell or face based models. It is ensured by assigning the value 'SurfaceModel' to the _RepresentationType_ attribute of _IfcShapeRepresentation_. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

**Brep Representation**  
Any _IfcElementComponent_ (if no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation elements (which are restricted to faceted Brep with or without voids). The Brep representation allows for the representation of complex element shape. It is ensured by assigning the value 'Brep' to the _RepresentationType_ attribute of _IfcShapeRepresentation_. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

**Mapped Representation**  
The mapped item, _IfcMappedItem_, should be used if appropriate as it allows for reusing the geometry definition of the equipment type at occurrences of the same equipement type. In this case the _IfcShapeRepresentation.RepresentationType_ = 'MappedRepresentation' is used.