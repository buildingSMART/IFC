The element type _IfcFlowFittingType_ defines a list of commonly shared property set definitions of a flow fitting and an optional set of product representations. It is used to define a flow fitting specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A flow fitting type is used to define the common properties of a flow fitting that may be applied to many occurrences of that type. A flow fitting is a device that is used to interconnect flow segments or other fittings within a distribution system, such as a tee in a ducted system that branches flow into two directions, a junction box in an electrical distribution system, etc. Flow fitting types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFlowFittingType_ are represented by instances of _IfcFlowFitting_ or its subtypes.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>