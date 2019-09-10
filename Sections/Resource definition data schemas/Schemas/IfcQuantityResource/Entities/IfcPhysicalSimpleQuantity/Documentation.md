The physical quantity, _IfcPhysicalSimpleQuantity_, is an entity that holds a single quantity measure value (as defined at the subtypes of _IfcPhysicalSimpleQuantity_) together with a semantic definition of the usage for the measure value.

> <font size="-1">EXAMPLE: An element, like a wall, may have
		several area measures, like footprint area, left wall face area, right wall
		face area. These areas would be given by three instances of the area quantity
		subtype, with different <i>Name</i> string values.</font>

A section "Quantity Use Definition" at individual entities as subtypes of _IfcBuildingElement_ gives guidance to the usage of the _Name_ attribute to characterize the individual quantities. If the _Unit_ attribute is given, the value attribute (introduced at the level of subtypes of _IfcPhysicalSimpleQuantity_) are given as quantities of this unit, otherwise the global unit definitions (given by _IfcUnitAssignment_) are used.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC Release 2x2
		  Addendum 1. </font>
>

> <font color="#FF0000" size="-1">IFC2x2 ADDENDUM 1 CHANGE The abstract
		  entity <i>IfcPhysicalSimpleQuantity</i> has been added. Upward compatibility
		  for file based exchange is guaranteed.</font>
>
