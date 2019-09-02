**Definition from ISO 10303-42:ed.2, 2000:** A rectangular pyramid is a solid pyramid with a rectangular base. The apex of the pyramid is directly above the centre point of the base. The rectangular pyramid is specified by its position, which provides a placement coordinate system, its length, depth and height.

&nbsp;The inherited _Position_ attribute defines the _IfcAxis2Placement3D_ and provides the location and orientation of the pyramid:

* _SELF\IfcCsgPrimitive3D.Position_:&nbsp;The position defines a placement coordinate system for the pyramid.
* _SELF\IfcCsgPrimitive3D.Position.Location_: The pyramid has one corner of its base at the location and the edges of the base are aligned with the first two placement axes in the positive sense.

<table border="0" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top"><a href="drawings/IfcRectangularPyramid-Layout1.dwf"><img alt="pyramid" src="figures/IfcRectangularPyramid-Layout1.png" border="0" height="300" width="400"></a></td>
      <td valign="top">The pyramid is positioned within
its
own placement coordinate system. One corner is at the origin,
and&nbsp;he values for <i>XLength</i>, and<i>
YLength</i> are
applied to the positive direction of the X, and Y axis. The apex is at [<i>XLength</i>/2,
      <i>YLength</i>/2, <i>Height</i>].</td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP entity: rectangular_pyramid, the position attribute
has been promoted to the immediate supertype <i>IfcCsgPrimitive3D</i>.
Please refer to ISO/IS 10303-42:1994, p. 246 for the final definition
of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC2x Edition 3.</font>
>