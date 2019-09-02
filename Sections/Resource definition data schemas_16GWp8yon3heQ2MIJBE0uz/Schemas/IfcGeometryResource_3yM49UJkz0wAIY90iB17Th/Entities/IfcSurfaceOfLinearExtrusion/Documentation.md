**Definition from ISO/CD 10303-42:1992**: This surface is a simple swept surface or a generalized cylinder obtained by sweeping a curve in a given direction. The parameterization is as follows where the curve has a parameterization <font face="Symbol">l</font>(_u_):

> 
>> V = ExtrusionAxis
>> 
>> ![Image](figures/IfcSurfaceOfLinearExtrusion-Math1.gif)
>>


> 
The parameterization range for _v_ is -<font face="Symbol">&yen;</font> &lt; _v_ &lt; <font face="Symbol">&yen;</font> and for _u_ it is defined by the curve parameterization.

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  surface_of_linear_extrusion. Please refer to ISO/IS 10303-42:1994, p.76 for the
		  final definition of the formal standard. The following adaption has been made.
		  The <i>ExtrusionAxis</i> and the <i>Direction</i> are defined as two separate
		  attributes in correlation to the definition of the extruded_area_solid, and not
		  as a single vector attribute. The vector is derived as
		  <i>ExtrusionAxis</i>.</font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2x.</font>
>

**Informal propositions**:

1. The surface shall not self-intersect