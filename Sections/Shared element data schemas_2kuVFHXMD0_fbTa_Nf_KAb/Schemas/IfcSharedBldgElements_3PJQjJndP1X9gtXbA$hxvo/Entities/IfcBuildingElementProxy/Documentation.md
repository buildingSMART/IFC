The _IfcBuildingElementProxy_ is a proxy definition that provides the same functionality as subtypes of _IfcBuildingElement_, but without having a predefined meaning of the special type of building element, it represents.

Proxies can also be used as spatial place holders or provisions, that maybe later replaced by special types of elements.

One use of the proxy object is a provision for voids, i.e. where a particular volume of space is requested by some engineering function that might later be accepted or rejected and if accepted potentially transformed into a void within a building element, like a wall opening, or a slab opening. The provision for voids is exchanged as an _IfcBuildingElementProxy_ with the _PredefinedType_ = ProvisionForVoid.

Other usages of _IfcBuildingElementProxy_ include:

* The _IfcBuildingElementProxy_ can be used to exchange special types of building elements for which the current specification does not yet provide a semantic definition.
* The _IfcBuildingElementProxy_ can also be used to represent building elements for which the participating applications can not provide a semantic definition.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _CompositionType_ has been replaced by _PredefinedType_, being a superset of the enumerators.