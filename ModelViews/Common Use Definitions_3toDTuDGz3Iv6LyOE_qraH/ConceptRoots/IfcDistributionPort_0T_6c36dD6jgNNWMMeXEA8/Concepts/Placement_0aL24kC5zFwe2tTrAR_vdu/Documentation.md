The placement of a port indicates the position and orientation of how it may connect to a compatible port on another product. The placement shall be relative to the nesting _IfcDistributionElement_, _IfcDistributionElementType_, or enclosing _IfcDistributionPort_.

The _Location_ is the midpoint of the physical connection, unless otherwise indicated by cardinal point on a material profile.

The _Axis_ points in the direction of the physical connection away from the product if _FlowDirection_ equals _SOURCE_ (or _SOURCEANDSINK_ or _NOTDEFINED_), or points opposite direction (to the product) if the _FlowDirection_ equals _SINK_.

> NOTE&nbsp; The rationale for positioning the _Axis_ in the direction of flow is to allow for the same geometry to be used, such as for connectors with polarized cross-section.

The _RefDirection_ points in the direction of the local X axis of the material profile, where the local Y axis points up if looking towards the _Axis_ where the local X axis points right.

Upon connecting elements through ports with rigid connections, each object shall be aligned such that the effective _Location_, _Axis_, and _RefDirection_ of each port is aligned to be equal (with exception for circular profiles where the _RefDirection_ need not be equal).