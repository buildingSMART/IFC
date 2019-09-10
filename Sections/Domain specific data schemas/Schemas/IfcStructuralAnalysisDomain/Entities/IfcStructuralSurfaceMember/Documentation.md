Instances of the entity _IfcStructuralSurfaceMember_ shall be used to describe planar structural elements.

The material properties are defined by _IfcMechanicalMaterialProperties_ (and subtypes) and they are connected through _IfcMaterial_ and _IfcRelAssociatesMaterial_ and are accessible via the inherited inverse relationship _HasAssociations_.

> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
> 


****Topology Use Definition****

Instances of _IfcStructuralSurfaceMember_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_".

**Placement**

The placement for _IfcStructuralSurfaceMember_ is determined at its supertype _IfcProduct_. It is defined by the optional _IfcObjectPlacement_, referenced by _ObjectPlacement_ at _IfcProduct_, which establishes, if given, the object coordinate system that is referenced by all topological representations of that product.

* If the _ObjectPlacement_ attribute is omitted, then all topological representations are given directly in world coordinates.
* If the _ObjectPlacement_ attribute is provided, then it establishes an object coordinate system for all topological representations which are given object coordinates. 
    * If the _PlacementRelTo_ relationship of _IfcLocalPlacement_ is omitted, the object coordinate system is established within the world coordinate system.
    * If the _PlacementRelTo_ relationship of _IfcLocalPlacement_ is given, it shall point to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 

**Topology Representation**

Instances of _IfcStructuralSurfaceMember_ shall have a topology representation given by a face with an optional additional geometric representation of the included surface. It can be provided by either

* _IfcFace_
* _IfcFaceSurface_

which should be the single item of _IfcTopologyRepresentation.Items_.
