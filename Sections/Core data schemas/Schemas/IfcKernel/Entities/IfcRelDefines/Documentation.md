A definition relationship (_IfcRelDefines_) that uses a type definition or property set definition (seens as partial type information) to define the properties of the object instance. It is a specific - occurrence relationship with implied dependencies (as the occurrence properties depend on the specific properties).

The _IfcRelDefines_ relationship establishes the link between one type (specific) information and several objects (occurrences). Those occurrences then share the same type (or partial type) information.

> <font size="-1">EXAMPLE: Several instances of windows within
		the IFC project model may be of the same (catalogue or manufacturer) type.
		Thereby they share the same properties. This relationship is established by a
		subtype of the <i>IfcRelDefines</i> relationship assigning an
		<i>IfcProductType</i> (or subtype thereof) to the
		<i>IfcWindow</i>.</font>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
		Release 2x.</font>
