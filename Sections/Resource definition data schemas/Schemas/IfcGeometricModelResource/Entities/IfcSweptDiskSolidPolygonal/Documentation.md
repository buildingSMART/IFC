The _IfcSweptDiskSolidPolygonal_ is a _IfcSweptDiskSolid_ where the _Directrix_ is restricted to be provided by an _IfcPolyline_ only. An optional _FilletRadius_ attribute can be asserted, it is then applied as a fillet to all transitions between the segments of the _IfcPolyline_.

> HISTORY&nbsp; New entity in IFC4.

{ .spec-head}
Informal Propositions:

1. The _FilletRadius_, if provided, has to be smaller then or equal to the length of the start and end segment of the _IfcPolyline_, and smaller then or equal to one half of the lenght of the shortest inner segment.
