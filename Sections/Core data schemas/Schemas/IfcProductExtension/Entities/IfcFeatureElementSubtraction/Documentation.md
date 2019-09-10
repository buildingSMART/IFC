A specialization of the general feature element, that represents an existence dependent elements which modifies the shape and appearance of the associated master element. The _IfcFeatureElementSubtraction_ offers the ability to handle shape modifiers as semantic objects within the IFC object model that subtract from the shape of the master element.

> <small><font color="#0000FF">HISTORY New entity in
        Release IFC2x Edition 2.</font></small>  
> <small><font color="#FF0000">NOTE The entity is
        introduced as an upward compatible extension of the IFC2x
        platform. It is an intermediate abstract supertype
        without defining its own explicit attributes. The
        existing <i>IfcOpeningElement</i> is subtyped from
        it.</font></small>
> 


****Containment use definition****

The containment to the spatial structure is defined at the level of the supertype _IfcFeatureElement_

****Geometry Use Definitions****

The geometric representation of _IfcFeatureElementSubtraction_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcFeatureElementSubtraction_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations. The local placement is always defined in relation to the local placement of the building element from which the feature element is substracted:

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcElement_, which is used in the _VoidsElements.RelatingElement_ inverse attribute. 

**Shape Representation**

The geometry use definitions for the shape representation of the _IfcFeatureElementSubtraction_ is given at the level of its subtypes.