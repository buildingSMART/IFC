The element type (_IfcCurtainWallType_) defines a list of commonly shared property set definitions of a curtain wall element and an optional set of product representations. It is used to define a curtain wall specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">NOTE: The product
representations are defined as representation maps (at the level of the
supertype <i>IfcTypeProduct</i>, which gets assigned by an
element occurrence instance through the <i>IfcShapeRepresentation.Item[1]</i>
being an <i>IfcMappedItem</i>.</font>
> 


A curtain wall type is used to define the common properties of a certain type of curtain wall that may be applied to many instances of that type to assign a specific style. Curtain wall types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcCurtainWallType_ are represented by instances of _IfcCurtainWall._

> <font color="#0000ff" size="-1">HISTORY
New entity in Release IFC2x Editon 3.</font>
>