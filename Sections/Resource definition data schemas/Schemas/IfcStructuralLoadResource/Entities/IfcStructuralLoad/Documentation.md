The abstract entity _IfcStructuralLoad_ is the supertype of all loads which can be defined (actions or reactions, as well as dynamic or static).

Subtypes of this entity are an important part of the definition of actions and reactions. They are used to specify the load values. The location and the used coordinate system are defined by instances of _IfcStructuralActivity_ which reference an instance of _IfcStructuralLoad_ for the definition of the load values. This offers the possibility to use instances of _IfcStructuralLoad_ by several instances of _IfcStructuralActivity_.

> <font size="-1">NOTE: Within the scope of this IFC release dynamic
		  loads are not considered, therefore only one subtype,
		  <i>IfcStructuralLoadStatic</i>, is defined. </font>
>

> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  edition 2. </font>
>