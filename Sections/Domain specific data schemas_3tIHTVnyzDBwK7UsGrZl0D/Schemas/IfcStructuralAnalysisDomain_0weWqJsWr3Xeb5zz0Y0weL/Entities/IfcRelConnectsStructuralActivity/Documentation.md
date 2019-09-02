The _IfcRelConnectsStructuralActivity_ relationship connects a structural activity (either an action or reaction) to a structural member or a building element.

> <font size="-1">NOTE: The use of this entity in the modelling
		of the mechanical structure of a building is optional. It is only needed to
		associate structural representations with structural actions. However, since
		the location of a structural action is defined by using a topology object -
		which is also used by the structural member on which it acts - the explicit
		association of activities to structural representations is not always
		necessary. It is possible to determine such connections by analysing the used
		topology. On the other hand, this is not unambiguous in all cases, as for
		example by eccentric loading. Furthermore, it may result in complicated
		operations for the detection of the needed references. Therefore the use of
		this entity is strongly recommended to avoid ambiguity.</font>

> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
>