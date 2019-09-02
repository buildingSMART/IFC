The _IfcBuildingElementProxyType_ defines a list of commonly shared property set definitions of a building element proxy and an optional set of product representations. It is used to define an element specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <small>NOTE  The product representations are defined as
        representation maps (at the level of the supertype
        <i>IfcTypeProduct</i>, which gets assigned by an element
        occurrence instance through the
        <i>IfcShapeRepresentation.Item[1]</i> being an
        <i>IfcMappedItem</i>.</small>
> 


A building element proxy type is used to define the common properties of a certain type of a building element proxy that may be applied to many instances of that type to assign a specific style. Building element proxy types may be exchanged without being already assigned to occurrences.

> <small>NOTE  Although an building element proxy does not have
		a predefined ontological meaning the provision of a type may be
		helpful in sharing information among multiple occurrences. Applications 
		that provide type information for element types not yet included in the
		current IFC specification can use the <i>IfcBuildingElementProxyType</i>
		to exchange such types.</small>
> 


The occurrences of the _IfcBuildingElementProxyType_ are represented by instances of _IfcBuildingElementProxy_.

> <font color="#0000FF"><small>HISTORY  New entity in
        Release IFC2x Edition 3.</small></font>
>