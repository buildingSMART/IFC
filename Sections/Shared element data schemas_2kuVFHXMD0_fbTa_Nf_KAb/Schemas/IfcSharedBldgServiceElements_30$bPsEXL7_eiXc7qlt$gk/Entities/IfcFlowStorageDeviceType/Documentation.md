The element type _IfcFlowStorageDeviceType_ defines a list of commonly shared property set definitions of a flow storage device and an optional set of product representations. It is used to define a flow storage device specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A flow storage type is used to define the common properties of a flow storage device that may be applied to many occurrences of that type. A flow storage device is a device used for the temporary storage of a fluid such as a liquid or a gas (e.g., tank), the voltage potential induced by the induced electron flow (e.g., a battery), etc. Flow storage types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFlowStorageDeviceType_ are represented by instances of _IfcFlowStorage_ or its subtypes.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>