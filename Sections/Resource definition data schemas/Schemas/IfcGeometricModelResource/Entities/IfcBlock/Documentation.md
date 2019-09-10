**Definition from ISO/CD 10303-42:1992:** A block is a solid rectangular parallelepiped, defined with a location and placement coordinate system. The block is specified by the positive lengths x, y, and z along the axes of the placement coordinate system, and has one vertex at the origin of the placement coordinate system.

&nbsp;The inherited _Position_ attribute defines the _IfcAxis2Placement3D_ and provides:

* _SELF\IfcCsgPrimitive3D.Position_: The location and orientation of the axis system for the primitive.&nbsp;
* _SELF\IfcCsgPrimitive3D.Position.Location_: The block has one vertex at location and the edges are aligned with the placement axes in the positive sense.

<table cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top"><a href="drawings/IfcBlock-Layout1.dwf"><img alt="block" src="figures/ifcblock-layout1.png" border="0" height="300" width="400"></a></td>
      <td valign="top">The block is positioned within its
own placement coordinate system. The values for <i>XLength</i>,
      <i>YLength</i>, and <i>ZLength</i> are
applied to the positive direction of the X, Y, and Z axis.</td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP entity: block, the position attribute has been
promoted to the immediate supertype <i>IfcCsgPrimitive3D</i>.
Please refer to ISO/IS 10303-42:1994, p. 244 for the final definition
of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC2x Edition 3.</font>
>
