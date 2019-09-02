The following restriction is imposed:

1. The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the same element (if given), in which the _IfcWindow_ is used as a filling (normally an _IfcOpeningElement_), as provided by the _IfcRelFillsElement_ relationship.
2. If the _IfcWindow_ is not inserted into an _IfcOpeningElement_, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
3. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

> NOTE&nbsp; The product placement is used to determine the opening direction of the window.