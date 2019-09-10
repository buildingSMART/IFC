**Definition from ISO/CD 10303-42:1992**: The trimmed surface is a simple bounded surface in which the boundaries are the constant parametric lines _u_~1~ = u1, _u_~2~ = u2, _v_~1~ = v1 and _v_~2~ = v2. All these values shall be within the parametric range of the referenced surface. Cyclic properties of the parameter range are assumed.

> NOTE 1 For example, 370 degrees is equivalent to 10 degrees, for those surfaces whose parametric form is defined using circular functions (sine and cosine).

The rectangular trimmed surface inherits its parameterization directly from the basis surface and has parameter ranges from 0 to |_u_~2~ - _u_~1~| and 0 to |_v_~2~-_v_~1~|.

> NOTE 2 If the surface is closed in a given parametric direction, the values of _u_~2~ or _v_~2~ may require to be increased by the cyclic range.

> <font color="#0000FF" size="-1"> NOTE Corresponding STEP name:
		  rectangular_trimmed_surface. Please refer to ISO/IS 10303-42:1994, p.86 for the
		  final definition of the formal standard. </font>
> 
> <font size="-1"><font color="#0000FF">HISTORY New class in IFC Release
		  2x.</font> </font>
>

**Informal propositions**:

1. The domain of the trimmed surface shall be within the domain of the surface being trimmed.