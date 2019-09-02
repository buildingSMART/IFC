**Definition from ISO/CD 10303-42:1992**: An offset curve 3d is a curve at a constant distance from a basis curve in three-dimensional space. The underlying curve shall have a well-defined tangent direction at every point. In the case of a composite curve the transition code between each segment shall be cont same gradient or cont same gradient same curvature. The offset curve at any point (parameter) on the basis curve is in the direction _V x T_ where _V_ is the fixed reference direction and _T_ is the unit tangent to the basis curve. For the offset direction to be well defined, _T_ shall not at any point of the curve be in the same, or opposite, direction as _V_.

> <font size="-1">NOTE: The offset curve 3d may differ in nature from
		  the basis curve; the offset of a non self- intersecting curve can be
		  self-intersecting. Care should be taken to ensure that the offset to a
		  continuous curve does not become discontinuous.</font>
>

The offset curve 3d takes its parameterization from the basis curve. The offset curve 3d is parameterized as

> ![Math](figures/IfcOffsetCurve3d-Math1.gif)
>

where **T** is the unit tangent vector to the basis curve **C**(_u_) at parameter value _u_, and _d_ is distance. The underlying curve shall be three-dimensional.

> <font size="-1" color="#0000FF">NOTE Corresponding STEP entity:
		  offset_curve_3d, Please refer to ISO/IS 10303-42:1994, p.66 for the final
		  definition of the formal standard. </font>
> 
> <font size="-1" color="#0000FF">HISTORY New entity in IFC Release 2.x
		  </font>
>

**Informal propositions:**

1. At no point on the curve shall ref direction be parallel, or opposite to, the direction of the tangent vector.