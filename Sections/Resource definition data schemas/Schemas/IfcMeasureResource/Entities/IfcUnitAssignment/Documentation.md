﻿_IfcUnitAssignment_ indicates a set of units which may be assigned. Within an _IfcUnitAssigment_ each unit definition shall be unique; that is, there shall be no redundant unit definitions for the same unit type such as length unit or area unit. For currencies, there shall be only a single _IfcMonetaryUnit_ within an _IfcUnitAssignment_.

> NOTE&nbsp; A _IfcProject_ has a unit assignment which establishes a set of units which will be used globally within the project, if not otherwise defined. Other objects may have local unit assignments if there is a requirement for them to make use of units which do not fall within the project unit assignment.

> HISTORY&nbsp; New entity in IFC1.5.1.
