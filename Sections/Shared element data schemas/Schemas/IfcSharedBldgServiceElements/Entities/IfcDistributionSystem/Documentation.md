﻿A distribution system is a network designed to receive, store, maintain, distribute, or control the flow of a distribution media. A common example is a heating hot water system that consists of a pump, a tank, and an interconnected piping system for distributing hot water to terminals.

The group _IfcDistributionSystem_ defines the occurrence of a specialized system for use within the context of building services or utilities for built facilities.

Important functionalities for the description of a distribution system are derived from existing IFC entities:

* From _IfcSystem_ it inherits the ability to couple the distribution system via _IfcRelServicesBuildings_ to one or more _IfcSpatialElement_ subtypes as necessary.

* From _IfcGroup_ it inherits the inverse attribute _IsGroupedBy_, pointing to the relationship entity _IfcRelAssignsToGroup_. This allows to group distribution elements (instances of _IfcDistributionElement_ subtypes), and in special cases ports directly (instances of _IfcDistributionPort_).

* From _IfcObject_ it inherits the inverse attribute _IsDecomposedBy_ pointing to the relationship entity _IfcRelAggregates_. It provides the hierarchy between the separate (partial) distribution systems. For example, an electrical main circuit may be aggregated into branch circuits.

> HISTORY&nbsp; New entity in IFC4.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; For electrical power systems, _IfcElectricalCircuit_ has been used for low-voltage (12-1000 V) power circuits and has been replaced by _IfcDistributionCircuit_ in IFC4; _IfcDistributionSystem_ with PredefinedType 'ELECTRICAL' should be used for overall power systems, and _IfcDistributionCircuit_ with PredefinedType 'ELECTRICAL' should be used for each switched circuit.
