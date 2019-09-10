**Definition from ISO/CD 10303-42:1992:** A sphere is a CSG primitive with a spherical shape defined by a centre and a radius.

&nbsp;The inherited _Position_ attribute defines the _IfcAxis2Placement3D_ and provides:

* _SELF\IfcCsgPrimitive3D.Position_: The location and orientation of the axis system for the primitive.&nbsp;
* _SELF\IfcCsgPrimitive3D.Position.Location_: The center of the sphere..
* _SELF\IfcCsgPrimitive3D.Position.Position[3]:_The z axis points at its positve direction towards the north pole, and by its negative directions towards the south pole.

<table cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top" width="420"><a href="drawings/IfcSphere-Layout1.dwf"><img alt="sphere" src="figures/ifcsphere-layout1.png" border="0" height="300" width="400"></a></td>
      <td colspan="1" rowspan="2" valign="top"><img alt="sphere" src="figures/ifcsphere.jpg" height="400" width="400"></td>
    </tr>
    <tr>
      <td valign="top" width="420">The sphere is
positioned within its
own placement coordinate system. The origin is the center of the
sphere.&nbsp;</td>
    </tr>
    <tr>
      <td colspan="2" rowspan="1" valign="top" width="420">When a texture is applied to a sphere, the
texture covers the entire surface, wrapping counterclockwise from the
back of the sphere (i.e., longitudinal arc intersecting the +Y axis)
when viewed from the top of the sphere. The texture has a seam at the
back where the X=0 plane intersects the sphere and Y values are
positive. Texture Transform affects the texture coordinates of the
Sphere
      <blockquote><small>NOTE &nbsp;see the Extensible
3D (<a href="http://www.web3d.org/x3d/specifications/ISO-IEC-19775-X3DAbstractSpecification/Part01/components/geometry3D.html#Sphere">X3D</a>)
definition for textures, please note, that all extrusions in IFC are
into the positve z axis, whereas in X3D there are into the positive y
axis.</small></blockquote>
      </td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP entity: sphere, the position attribute, including
the centre point,&nbsp; has been promoted to the immediate
supertype <i>IfcCsgPrimitive3D</i>. Please refer to ISO/IS
10303-42:1994, p. 175 for the final definition of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC2x Edition 3.</font>
>
