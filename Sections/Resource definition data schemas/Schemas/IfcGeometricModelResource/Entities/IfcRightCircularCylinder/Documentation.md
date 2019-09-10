**Definition from ISO/CD 10303-42:1992:** A right circular cylinder is a CSG primitive in the form of a solid cylinder of finite height. It is defined by an axis point at the centre of one planar circular face, an axis, a height, and a radius. The faces are perpendicular to the axis and are circular discs with the specified radius. The height is the distance from the first circular face centre in the positive direction of the axis to the second circular face centre.

&nbsp;The inherited _Position_ attribute defines the _IfcAxis2Placement3D_ and provides:

* _SELF\IfcCsgPrimitive3D.Position_: The location and orientation of the axis system for the primitive.&nbsp;
* _SELF\IfcCsgPrimitive3D.Position.Location_: The center of the&nbsp;circular area being the bottom face of the cylinder.
* _SELF\IfcCsgPrimitive3D.Position.Position[3]:_The z axis provides the center axis and the height is measured from the origin along the positive direction of the z axis.

<table border="0" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top" width="420"><img alt="cylinder" src="figures/ifcrightcircularcylinder-layout1.png" height="300" width="400"></td>
      <td colspan="1" rowspan="2" valign="top"><img alt="cylinder" src="figures/ifcrightcircularcylinder.jpg" height="400" width="400"></td>
    </tr>
    <tr>
      <td width="420">The cylinder is positioned within
its
own placement coordinate system. The origin is the center of the bottom
circular disk, that lies in the XY plane. The center of the top
circular disk is on the positive z axis at [0, 0, <i>Height</i>].</td>
    </tr>
    <tr>
      <td colspan="2" rowspan="1" width="420">When
a texture is applied to a cylinder, it is applied differently to the
sides, top, and bottom. On the sides, the texture wraps
counterclockwise (from above) starting at the back of the cylinder. The
texture has a vertical seam at the back, intersecting the X=0 plane,
from (0, <i>Radius</i>, 0) to (0, <i>Radius</i>,
      <i>Height</i>). For the top and bottom caps, a circle
is cut out of the unit texture squares centred at bottom (0, 0, 0) and
top (0, 0, <i>Height</i>) with dimensions
2&nbsp;&times; <i>Radius</i> by
2&nbsp;&times; <i>Radius</i>. The top texture
appears right side up when the top of the cylinder is tilted toward the
+Z-axis, and the bottom texture appears right side up when the top of
the cylinder is tilted toward the &minus;Z-axis. TextureTransform
affects the texture coordinates of the Cylinder node <br>
      <blockquote><small>NOTE &nbsp;see the Extensible
3D (<a href="http://www.web3d.org/x3d/specifications/ISO-IEC-19775-X3DAbstractSpecification/Part01/components/geometry3D.html#Cylinder">X3D</a>)
definition for textures, please note, that all extrusions in IFC are
into the positve z axis, whereas in X3D there are into the positive y
axis, and the IFC cylinder is positioned at the bottom face, whereas in
X3D it is positioned centric..</small></blockquote>
      </td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP entity: right_circular_cylinder, the position
attribute has been promoted to the immediate supertype <i>IfcCsgPrimitive3D</i>.
Please refer to ISO/IS 10303-42:1994, p. 177 for the final definition
of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC2x Edition 3.</font>
>
