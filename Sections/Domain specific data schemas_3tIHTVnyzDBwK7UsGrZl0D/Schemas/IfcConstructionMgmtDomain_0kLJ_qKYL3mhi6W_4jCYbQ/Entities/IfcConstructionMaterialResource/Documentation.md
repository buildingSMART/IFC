An _IfcConstructionMaterialResource_ identifies a material resource type in a construction project.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0 </font>

### Use Definition
Occurrences of IfcConstructionMaterialResource are consumed (wholly or partially), or occupied during a construction work task (i.e. _IfcTask_).

Similar to _IfcConstructionProductResource_, sometimes things such as 5000kg of gravel are already instantiated as an IfcProduct because it is a result of a work task e.g. &#145;transporting gravel&#146;. In this case, the instance of _IfcConstructionMaterialResource_ can be associated with the product instance &#145;5000kg of gravel&#146; to provide more information for resource uses. Nevertheless, _IfcConstructionMaterialResource_ should only be used to represent resource types, e.g. &#145;gravel&#146;, but not product substances, e.g. &#145;5000kg of gravel&#146;.

Note: This class is not the same as _IfcMaterial_; the former can typically represent the type of bulk materials such as sand, gravels, nails and so on (note these can be instantiated from _IfcProduct_ as well depending their uses in the system) used in a construction process. The latter is about physical materials used in a physical building element typically with detailed positioning (e.g. offset) and layering information.

The association of an actual material with an _IfcConstructionMaterialResource_ is handled by _IfcRelAssociatesMaterial_.

Quantities for an _IfcConstructionMaterialResource_ are defined through _IfcRelDefinesByProperty_ and use _IfcElementQuantity_.