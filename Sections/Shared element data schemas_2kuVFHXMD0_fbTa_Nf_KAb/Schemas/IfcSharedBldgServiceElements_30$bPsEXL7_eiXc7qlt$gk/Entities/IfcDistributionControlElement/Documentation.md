The distribution element _IfcDistributionControlElement_ defines occurrence elements of a building automation control system that are used to impart control over elements of a distribution system.

This class defines elements of a building automation control system. These are typically used to control distribution system elements to maintain temperature, humidity, pressure, flow, power, lighting levels, etc., through the modulation, staging or sequencing of mechanical or electrical devices. The three general functional categories of ControlElements as defined for this release of the IFC model are as follows:

* Impart control over flow control elements (_IfcFlowController_) in a distribution system such as dampers, valves, relays, etc., typically through the use of actuation (_IfcActuator_: See _IfcHvacDomain_ schema).
* Sensing elements (_IfcSensor_: See _IfcHvacDomain_ schema) that measure changes in the controlled variable (e.g., temperature, humidity, pressure, flow, etc.).
* Controllers (_IfcController_: See _IfcHvacDomain_ schema) typically classified according to the control action they seek to perform and generally responsible for making decisions about the elements under control.

Since this class and its subtypes typically relate to many different distribution flow elements (_IfcDistributionFlowElement_), the objectified relationship _IfcRelFlowControlElements_ has been provided to relate control and flow elements as required.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0.<br>
    	</font>

**Geometry Use Definitions**

The geometric representation of _IfcControlElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The local placement is defined in the supertype _IfcProduct_. It is defined by a subtype of _IfcObjectPlacement_ which can define an absolute placement, relative placement, or grid reference, with each defining the local coordinate system referenced by all geometric representations. The PlacementRelTo relationship of _IfcLocalPlacement_, if given, shall point to the same _IfcSpatialStructureElement_ which is used in the ContainedInStructure inverse attribute, or to a referenced spatial structure element at a higher level. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**Informal propositions for local placement**:

1. If the LocalPlacement is specified, then all aggregated components should use this placement as their relative placement.

**Standard Geometric Representation**

Currently, the use of attribute driven geometry for this class is not supported. The standard geometric representation is defined using explicit geometry.

**B-Rep Representation**

The faceted B-Rep capabilities (with or without voids) shall be supported for B-Rep representation.