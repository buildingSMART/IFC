The assignment relationship, _IfcRelAssigns_, is a generalization of "link" relationships among instances of IfcObject and its various 1^st^ level subtypes. A link denotes the specific association through which one object (the client) applies the services of other objects (the suppliers), or through which one object may navigate to other objects.

The client is denoted as the relating object and is established at the level of the specific, instantiable subtypes of _IfcRelAssigns_. The suppliers are denoted as the related objects and they are established by the _RelatedObjects_ attribute.

> <font size="-1">NOTE: The terms "client" and "supplier" are
		used in a general concept and do not imply any meaning for implementations of
		systems (like client-server).</font>

> <font size="-1">EXAMPLE: A resource may receive information
		about its nature of representing real building products by establishing a link
		between <i>IfcResource</i> and <i>IfcBuildingElement</i> (subtype of
		<i>IfcProduct</i>) throught he assignment relationship
		<i>IfcRelAssignsToResource</i>. The resource is then the client that applies
		the services of other objects (here building elements) to express the
		particular view of elements to be consumed as a resource in a
		process.</font>

The assignment relationship establishs a bi-directional relationship among the participating objects and does not imply any dependency. The subtypes of IfcRelAssigns establishes the particular semantic meaning of the assignment relationship.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2x.</font>
>
