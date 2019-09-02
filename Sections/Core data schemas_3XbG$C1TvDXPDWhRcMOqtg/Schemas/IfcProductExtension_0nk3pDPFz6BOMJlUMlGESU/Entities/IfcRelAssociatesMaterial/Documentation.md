Objectified relationship between a material definition and elements or element types to which this material definition applies. The material definition can be:

* A single material 
* A material list, e.g. for composite elements 
* A material layer set, for layered elements with an indication of the layering direction and individual layer thicknesses 
* A material layer set usage, i.e. a material layer set with positioning information along the reference axis or surface of the element.

The _IfcRelAssociatesMaterial_ relationship is a special type of the _IfcRelAssociates_ relationship. It can be applied to subtypes of _IfcElement_ and subtypes of _IfcElementType_.

* The _IfcElement_ has an inverse relation to its material definition by the _HasAssociations_ attribute, inherited from _IfcObject_. 
* The _IfcElementType_ has an inverse relation to its material definition by the _HasAssociations_ attribute, inherited from _IfcPropertyDefinition_. 

If both, the element occurrence (by an instance of _IfcElement_) and the element type (by an instance of _IfcElementType_, connected through _IfcRelDefinesByType_) have an associated material, then the material associated to the element occurrence overrides the material associated to the element type.

> <small><font color="#0000FF">HISTORY New entity in IFC
        Release 2.x.</font></small>
> 


**Informal proposition**

1. An _IfcMaterialLayerSetUsage_ shall not be associated with a subtype of _IfcElementType_, it should only be associated with individual occurrences