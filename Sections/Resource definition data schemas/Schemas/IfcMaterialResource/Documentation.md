The schema _IfcMaterialResource_ contains the types and classes which are used to define materials. Materials are defined generically, with references to the usage of materials being made from the relevant classes through an objectified relationship.

Material designation can be made using

1.  a single material _IfcMaterial_,
2.  a list of materials (without a specified configuration or structure) _IfcMaterialList_, or 
3.  a structured set of material layers _IfcMaterialLayerSetUsage_.

These three options are exposed for association with _IfcElement_ through a select type _IfcMaterialSelect_, but some may be ruled out as appropriate in the specialized element subtypes.

> <font size="-1">NOTE: Definition of material properties and their assignment to <i>IfcMaterial</i> are captured in <i>IfcMaterialPropertyResource</i> schema.</font>

> <font size="-1" color="#0000FF">HISTORY New schema in IFC Release 2.0.</font>
