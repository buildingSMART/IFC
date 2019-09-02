**Definition from ISO/CD 10303-43:1992**: A representation map is the identification of a representation and a representation item in that representation for the purpose of mapping. The representation item defines the origin of the mapping. The representation map is used as the source of a mapping by a mapped item.

> <font size="-1">NOTE: The definition of a mapping which is used to
		  specify a new representation item comprises a representation map and a mapped
		  item entity. Without both entities, the mapping is not fully defined. Two
		  entities are specified to allow the same source representation
		  (representation.map.mapped_representation) to be mapped into multiple new
		  representations (mapped_item) </font>
>

An _IfcRepresentationMap_ defines the base definition (also referred to as block, cell or macro) within the mapping origin, defined as the placement coordinate system. The representation map is restricted to Cartesian mapping.

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  representation_map. Please refer to ISO/IS 10303-43:1994, for the final
		  definition of the formal standard. The following changes have been made: The
		  mapping_origin (<i>MappingOrigin</i>) is constrained to be of type
		  axis2_placement (<i>IfcAxis2Placement</i>). </font>
> 
> <font size="-1" color="#0000FF">HISTORY: New entity in IFC Release
		  2x.</font>
>