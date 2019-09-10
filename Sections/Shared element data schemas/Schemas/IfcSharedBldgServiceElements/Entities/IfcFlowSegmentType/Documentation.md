The element type _IfcFlowSegmentType_ defines a list of commonly shared property set definitions of a flow segment and an optional set of product representations. It is used to define a flow segment specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A flow segment type is used to define the common properties of a flow segment that may be applied to many occurrences of that type. A flow segment is a section of a distribution system, such as a duct, pipe, conduit, etc. that typically has only two ports. Flow segment types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFlowSegmentType_ are represented by instances of _IfcFlowSegment_ or its subtypes.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
