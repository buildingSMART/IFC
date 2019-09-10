A set of units which may be assigned. Within an _IfcUnitAssigment_ each unit definition shall be unique. I.e. there shall be no redundant unit definitions for the same unit type, like length unit, area unit etc. For currencies, there shall be only a single _IfcMonetaryUnit_ within an _IfcUnitAssignment_.

> <small>
NOTE&nbsp; A project (<i>IfcProject</i>) has a unit
assignment which establishes a set of units which will be used globally
within the project, if not otherwise defined. Other objects may have
local unit assignments if there is a requirement for them to make use
of units which do not fall within the project unit assignment.</small>

> <font color="#0000ff"><small>
HISTORY&nbsp; New entity in IFC Release 1.5.1.</small>
  </font>