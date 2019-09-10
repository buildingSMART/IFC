A specialization of the general feature element, that represents an existence dependent element which modifies the shape and appearance of the associated master element. The _IfcFeatureElementAddition_ offers the ability to handle shape modifiers as semantic objects within the IFC object model that add to the shape of the master element.

> <small><font color="#0000FF">HISTORY New entity in
        Release IFC2x Edition 2.</font></small>  
> <small><font color="#FF0000">NOTE The entity is
        introduced as an upward compatible extension of the IFC2x
        platform. It is an intermediate abstract supertype
        without defining its own explicit
        attributes.</font></small>
> 


The _IfcFeatureElementAddition_ is associated to its master element by virtue of the objectified relationship _IfcRelProjectsElement_. This relationship implies a Boolean 'union' operation between the shape of the master element and the shape of the addition feature.

****Containment use definition****

The containment to the spatial structure is defined at the level of the supertype _IfcFeatureElement_

****Geometry Use Definitions****

The geometric representation of _IfcFeatureElementAddition_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcFeatureElementAddition_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations. The local placement is always defined in relation to the local placement of the element to which the feature element is added:

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the same _IfcElement_, which is used in the _HasAdditionFeature.RelatingElement_ inverse attribute. 

**Shape Representation**

The geometry use definitions for the shape representation of the _IfcFeatureElementAddition_ is given at the level of its subtypes.
