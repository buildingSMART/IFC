Generalization of all equipment related objects, those objects are characterized as being pre-manufactured and being movable, and which provide some building service related or other servicing function. The term fixture is often used as a synonym or similar concept. The _IfcEquipmentElement_ covers the fixture aspect as well.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
      Release 2x</font>

> <font color="#FF0000" size="-1">IFC2x2 NOTE: The entity
      <i>IfcEquipmentElement</i> is deprecated and shall no
      longer be used.</font>

> <font size="-1">NOTE: The concept of equipment, that has a
      distribution function, such as electrical equipment, is now
      handled as distribution elements and class definitions are
      provided by subtypes of <i>IfcDistributionElement</i> for
      occurrences and <i>IfcDistributionElementType</i> for
      types. Equipment, that has no distribution function, is now
      handled within the <i>IfcSharedComponentElements</i>
      schema.</font>

**Geometry Use Definitions**:

The geometric representation of _IfcEquipmentElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcEquipmentElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ , which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**SurfaceModel Representation**

Any _IfcEquipmentElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple surface models, based on either shell or face based models. It is ensured by assigning the value 'SurfaceModel' to the RepresentationType attribute of _IfcShapeRepresentation_. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

**Brep Representation**

Any _IfcEquipmentElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation elements (which are restricted to faceted Brep with or without voids). The Brep representation allows for the representation of complex element shape. It is ensured by assigning the value 'Brep' to the RepresentationType attribute of _IfcShapeRepresentation_. In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

**MappedRepresentation**

The new mapped item, _IfcMappedItem_, should be used if appropriate as it allows for reusing the geometry definition of the equipment type at occurrences of the same equipment type. In this case the _IfcShapeRepresentation.RepresentationType_ = MappedRepresentation is used.
