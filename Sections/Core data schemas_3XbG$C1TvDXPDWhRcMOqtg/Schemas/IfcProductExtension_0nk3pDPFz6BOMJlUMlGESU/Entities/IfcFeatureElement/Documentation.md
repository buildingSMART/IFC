Generalization of all existence dependent elements which modify the shape and appearance of the associated master element. The _IfcFeatureElement_ offers the ability to handle shape modifiers as semantic objects within the IFC object model.

> <small>NOTE The term "feature" has a predefined meaning
        in a context of "feature-based modeling" and within steel
        construction work. It is introduced here in a broader
        sense to cover all existence dependent, but semantically
        described, modifiers of an element's shape and
        appearance. It is envisioned that future releases enhance
        the feature-based capabilities of the IFC model.</small>
> 


In contrary to the aggregation, as used in _IfcElementAssembly_, that defines the aggregate as a container element, that has equally treated parts, the feature concept introduced by _IfcFeatureElement_ defines the master element with subordinate parts as additions, or with voids or cut-outs as subtractions.

> <small><font color="#0000FF">HISTORY New entity in
        Release IFC2x Edition 2.</font></small>  
> <small><font color="#FF0000">NOTE The entity is
        introduced as an upward compatible extension of the IFC2x
        platform. It is an intermediate abstract supertype
        without defining its own explicit
        attributes.</font></small>
> 


****Containment Use Definition****

As a subordinate part being fully dependent on the master element the _IfcFeatureElement_ shall have no independent containment relationship to the spatial structure.

* The _SELF\IfcElement.ContainedInStructure_ relationship shall be NIL. 

****Geometry Use Definition****

The geometric representation of _IfcFeatureElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcFeatureElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the master _IfcElement_ (its relevant subtypes), which is associated to the _IfcFeatureElement_ by the appropriate relationship object. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**Shape Representation**

The geometry use definitions for the shape representation of the _IfcFeatureElement_ is given at the level of its subtypes.