**Definition from ISO/CD 10303-42:1992**: A placement entity defines the local environment for the definition of a geometry item. It locates the item to be defined and, in the case of the axis placement subtypes, gives its orientation.

**Additional definition from ISO/WD SC4/WG12/N071 Part42.2
		geometry_schema**: A placement locates a geometric item with respect to the coordinate system of its geometric context.

The _IfcPlacement_ is an abstract supertype not to be directly instantiated, whereas the STEP P42 entity placement can be instantiated to define a placement without orientation. The derived attribute _Dim_ has been added, see also note at _IfcGeometricRepresentationItem_.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  placement. Please refer to ISO/IS 10303-42:1994, p. 27 for the final definition
		  of the formal standard. </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 1.0
		  </font>
>