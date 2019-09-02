The complex physical quantity, _IfcPhysicalComplexQuantity_, is an entity that holds a set of single quantity measure value (as defined at the subtypes of _IfcPhysicalSimpleQuantity_), that all apply to a given component or aspect of the element.

> <font size="-1">EXAMPLE: A layered element, like a wall, may
		have several material layers, each having individual quantities, like footprint
		area, side area and volume. An instance of <i>IfcPhysicalComplexQuantity</i>
		would group these individual quantities (given by a subtype of
		<i>IfcPhysicalSimpleQuantity</i>) and name them according to the material layer
		name by using the <i>Name</i> attribute. The <i>Discrimination</i> attribute
		would then be 'layer'.</font>

A section "Quantity Use Definition" at individual entities as subtypes of _IfcBuildingElement_ gives guidance to the usage of the _Name_ and _Discrimination_ attribute to characterize the complex quantities.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC Release 2x2
		  Addendum 1. </font>
>

> <font color="#FF0000" size="-1">IFC2x2 ADDENDUM 1 CHANGE The entity
		  <i>IfcPhysicalComplexQuantity</i> has been added. Upward compatibility for file
		  based exchange is guaranteed.</font>
>