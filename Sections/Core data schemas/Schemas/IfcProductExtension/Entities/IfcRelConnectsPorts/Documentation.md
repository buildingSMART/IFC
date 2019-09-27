﻿An _IfcRelConnectsPorts_ relationship defines the relationship that is made between two ports at their point of connection. It may include the connection geometry between two ports.

The objectified relationship _IfcRelConnectsPorts_ is required for defining how two instances of _IfcPort_ connect together. Each of the ports is logically contained within the _IfcDistributionElement_ by using the ordered collection _IfcRelNests_.

> HISTORY&nbsp; New entity in IFC2.0, modified in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Previously the containment of the _IfcPort_ within the _IfcDistributionElement_ had been realized using the _IfcRelConnectsPortToElement_ relationship.
