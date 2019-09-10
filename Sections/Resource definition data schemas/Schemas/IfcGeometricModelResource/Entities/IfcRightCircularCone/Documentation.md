**Definition from ISO/CD 10303-42:1992:** A right circular cone is a CSG primitive in the form of a cone. It is defined by an axis, a point on the axis, (...) and a distance giving the location along the axis from the point to the base of the cone. In addition, a radius is given (...).

&nbsp;In contrary to the ISO/CD 10303-42 definition, the _IfcRightCircularCone_ may not be truncated. It provides:

* _SELF\IfcCsgPrimitive3D.Position_: The location and orientation of the axis system for the primitive.&nbsp;
* _SELF\IfcCsgPrimitive3D.Position.Location_: The center of the&nbsp;circular area being the bottom face of the cylinder.
* _SELF\IfcCsgPrimitive3D.Position.Position[3]:_The z-axis of the inherited placement coordinate system provides the center axis of the&nbsp;_IfcRightCircularCone_, and the apex is at the _Height_ value applied to the positive direction of the z-axis. The _BottomRadius_ defines the circular base at the xy-plane of the&nbsp;placement coordinate system.&nbsp;_&nbsp;_

_<table border="0" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top" width="420"><img alt="cone" src="figures/ifcrightcircularcone-layout1.png" height="300" width="400"></td>
      <td colspan="1" rowspan="2" valign="top"><img alt="cone" src="figures/ifcrightcircularcone.jpg" height="400" width="400"></td>
    </tr>
    <tr>
      <td valign="top" width="420">The cone is
positioned within its
own placement coordinate system. The origin is the center of the bottom
circular disk, that lies in the XY plane. The apex lies on the positive
z axis at [0, 0, <i>Height</i>].</td>
    </tr>
    <tr>
      <td colspan="2" rowspan="1" valign="top" width="420">When a texture is applied to the sides of the
cone, the texture wraps counterclockwise (from above) starting at the
back of the cone. The texture has a vertical seam at the back in the
X=0 plane, from the apex (0,&nbsp;0, <i>Height</i>) to
the point (0, <i>BottomRadius</i>, 0). For the bottom cap,
a circle is cut out of the texture square centred at (0, 0,&nbsp;0)
with dimensions (2&nbsp;&times; <i>BottomRadius)</i>
by (2&nbsp;&times; <i>BottomRadius)</i>. The
bottom cap texture appears right side up when the top of the cone is
rotated towards the -Z-axis. Texture Transform affects the texture
coordinates of the Cone.&nbsp;
      <blockquote><small>NOTE &nbsp;see the Extensible
3D (<a href="http://www.web3d.org/x3d/specifications/ISO-IEC-19775-X3DAbstractSpecification/Part01/components/geometry3D.html#Cone">X3D</a>)
definition for textures, please note, that all extrusions in IFC are
into the positve z axis, whereas in X3D there are into the positive y
axis, and the IFC cone is positioned at the bottom face, whereas in
X3D it is positioned centric..</small></blockquote>
      </td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP entity: right_circular_cone, the position attribute
has been promoted to the immediate supertype <i>IfcCsgPrimitive3D</i>.
No semi_angle attribute, and the radius defines the bottom radius,
since only a non-truncated cone is in scope. Please refer to ISO/IS
10303-42:1994, p. 176 for the final definition of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC2x Edition 3.</font>
>
