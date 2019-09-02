**Definition from ISO/CD 10303-42:1992**: An offset curve 2d (IfcOffsetCurve2d) is a curve at a constant distance from a basis curve in two-dimensional space. This entity defines a simple plane-offset curve by offsetting by distance along the normal to basis curve in the plane of basis curve. The underlying curve shall have a well-defined tangent direction at every point. In the case of a composite curve, the transition code between each segment shall be cont same gradient or cont same gradient same curvature.

> <font size="-1">NOTE: The offset curve 2d may differ in nature from
		  the basis curve; the offset of a non self- intersecting curve can be
		  self-intersecting. Care should be taken to ensure that the offset to a
		  continuous curve does not become discontinuous.</font>
>

The offset curve 2d takes its parameterization from the basis curve. The offset curve 2d is parameterized as

> ![Math](figures/IfcOffsetCurve2d-Math1.gif)
>

where **T** is the unit tangent vector to the basis curve **C**(_u_) at parameter value _u_, and _d_ is distance. The underlying curve shall be two-dimensional.

> <font size="-1" color="#0000FF">NOTE Corresponding STEP entity:
		  offset_curve_2d, Please refer to ISO/IS 10303-42:1994, p.65 for the final
		  definition of the formal standard. </font>
> 
> <font size="-1" color="#0000FF">HISTORY New entity in IFC Release 2.x
		  </font>
>