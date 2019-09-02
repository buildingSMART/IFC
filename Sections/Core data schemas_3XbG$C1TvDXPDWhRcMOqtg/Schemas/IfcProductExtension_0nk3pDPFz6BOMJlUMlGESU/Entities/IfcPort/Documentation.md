An _IfcPort_ provides the means for an element to connect to other elements.

An _IfcPort_ is associated with an _IfcElement_, it belongs to through the objectified relationship _IfcRelNests_ if such port is fixed, or _IfcRelConnectsPortToElement_ if such port is dynamically attached. Exactly two ports, belonging to two different elements, are connected with each other through the objectified relationship _IfcRelConnectsPorts_.

An instance of _IfcElement_ may have one or more points at which it connects to other instances of _IfcElement_. An instance of _IfcPort_ is located at a point where a connection can occur. The location of the port is determined in the context of the local coordinate system of the element to which it belongs.

> HISTORY&nbsp; New entity in IFC2x2.

{ .use-head}
Containment Use Definitions

As a subordinate part being fully dependent on the master element the _IfcPort_ shall have no independent containment relationship to the spatial structure.

{ .use-head}
Geometry Use Definition

The geometric representation of _IfcPort_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcPort_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the master _IfcElement_ or _IfcElementType_ (relevant subtypes), which is related to the _IfcPort_ by the relationship object _IfcRelNests_ for fixed ports, or _IfcRelConnectsPortToElement_ for dynamic ports. 

**Shape Representation**

The geometry use definitions for the shape representation of the _IfcPort_ is given at the level of its subtypes.