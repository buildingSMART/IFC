**Definition from ISO/CD 10303-42:1992**: This select type identifies all those types of entities which may participate in a Boolean operation to form a CSG solid.

CSG primitives are out of scope for the current IFC Release. Only faceted B-reps, swept area solids and half space solids are available as Boolean operands. Boolean results themselves can be used as operands thus enabling nested Boolean operations.

> <font color="#0000FF" size="-1">NOTE Corresponding STEP type:
		  boolean_operand, please refer to ISO/IS 10303-42:1994, p.167 for the final
		  definition of the formal standard. In IFC Release 1.5.1 &amp; 2.0 only Boolean
		  results (<i>IfcBooleanResult</i>), half space solids
		  (<i>IfcHalfSpaceSolid</i>), faceted B-Rep, extruded solids and revolved solids
		  (<i>IfcSolidModel</i>) are defined for being valid Boolean operands.
		  </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New Type in IFC Release 1.5.1
		  </font>
>
