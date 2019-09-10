An _IfcPort_ provides the means for an element to connect to other elements.

An _IfcPort_ is associated with an _IfcElement_, it belongs to, through the objectified relationship _IfcRelConnectsPortToElement_. Exactly two ports, belonging to two different elements, are connected with each other through the objectified relationship _IfcRelConnectsPorts_.

An instance of _IfcElement_ may have one or more points at which it connects to other instances of _IfcElement_. An instance of _IfcPort_ is located at a point where a connection can occur. The location of the port is determined in the context of the local coordinate system of the element to which it belongs.

> <small><font color="#0000FF">HISTORY New entity in
        Release IFC2x Edition 2.</font></small>
> 


****Containment Use Definitions****

As a subordinate part being fully dependent on the master element the _IfcPort_ shall have no independent containment relationship to the spatial structure.

****Geometry Use Definition****

The geometric representation of _IfcPort_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcPort_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the master _IfcElement_ (its relevant subtypes), which is associated to the _IfcPort_ by the relationship object _IfcRelConnectsPortToElement_. 

**Shape Representation**

The geometry use definitions for the shape representation of the _IfcPort_ is given at the level of its subtypes.
