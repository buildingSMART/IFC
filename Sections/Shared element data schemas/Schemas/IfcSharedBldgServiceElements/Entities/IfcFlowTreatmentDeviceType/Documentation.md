The element type _IfcFlowTreatmentDeviceType_ defines a list of commonly shared property set definitions of a flow treatment device and an optional set of product representations. It is used to define a flow treatment device specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A flow treatment type is used to define the common properties of a flow treatment device that may be applied to many occurrences of that type. A flow treatment device is a device used to change the physical properties of the medium, such as an air, oil or water filter (used to remove particulates from the fluid), duct silencer (used to attenuate noise), etc. flow treatment types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFlowTreatmentDeviceType_ are represented by instances of _IfcFlowTreatmentDevice_ or its subtypes.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
