**Definition from ISO/CD 10303-42:1992**: The curve bounded surface is a parametric surface with curved boundaries defined by one or more boundary curves. The bounded surface is defined to be the portion of the basis surface in the direction of N x T from any point on the boundary, where N is the surface normal and T the boundary curve tangent vector at this point. The region so defined shall be arcwise connected.

The _IfcCurveBoundedPlane_ is a specialized bounded surface class that deals only with bounding basis plane surfaces. The definition varies from STEP as outer and inner boundaries are separated attributes and refer to _IfcCurve_. The only basis surface that is allowed is of type _IfcPlane_, and the implicit_outer attribute has not been incorporated, since only unbounded surfaces are used as basis surface.

The _BasisSurface_ is an _IfcPlane_ that establishes the position coordinate system by _SELF\IfcElementarySurface.Position_. The _OuterBoundary_ and the _InnerBoundaries_ (if provided) shall lie on the surface of _IfcPlane_. Therefore the _IfcCurve_'s establishing the outer and inner boundaries shall be:

* either a 2D curve within the XY plane of the position coordinate sytem of _IfcPlane_
* or a 3D curve with all coordinates having a z value = 0.

> <font color="#0000ff"><small>NOTE
Corresponding STEP entity curve_bounded_surface has been changed to
meet the specific requirements of an easy representation of curve
bounded planes.</small> </font>
> 
> <font color="#0000ff"><small>HISTORY
&nbsp;New entity in IFC Release 1.5</small> </font>  
> <font color="#ff0000"><small>IFC2x
PLATFORM CHANGE: The data type of the attribute <i>OuterBoundary</i>
and <i>InnerBoundaries</i> has been changed from <i>Ifc2DCompositeCurve</i>
to its supertype <i>IfcCurve</i> with upward compatibility
for file based exchange.</small> </font>
>
