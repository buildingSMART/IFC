**Definition
from ISO/CD 10303-42:1992**: The location and orientation in three dimensional space of three mutually perpendicular axes. An axis2_placement_3D is defined in terms of a point (inherited from placement supertype) and two (ideally orthogonal) axes. It can be used to locate and originate an object in three dimensional space and to define a placement coordinate system. The entity includes a point which forms the origin of the placement coordinate system. Two direction vectors are required to complete the definition of the placement coordinate system. The axis is the placement Z axis direction and the ref_direction is an approximation to the placement X axis direction.

If the attribute values for _Axis_ and _RefDirection_ are not given, the placement defaults to P[1] (x-axis) as [1.,0.,0.], P[2] (y-axis) as [0.,1.,0.] and P[3] (z-axis) as [0.,0.,1.].&nbsp;

> <font color="#0000ff" size="-1">NOTE&nbsp;
Corresponding STEP name: axis2_placement_3d, please refer to ISO/IS
10303-42:1994 for the final definition of the formal standard. The WR5
is added to ensure that either both attributes <i>Axis</i>
and <i>RefDirection</i> are given, or both are omitted.<br>
  </font>
> 


> <font color="#0000ff" size="-1">HISTORY&nbsp;
New entity in IFC Release 1.5.</font>
> 


**Illustration**

<table cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td><a href="drawings/IfcAxis2Placement3D-Layout1.dwf"><img src="figures/IfcAxis2Placement3D-Layout1.gif" alt="axis2 placement 2D" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top"><font size="-1">Definition of the <i>IfcAxis2Placement3D</i>
within the three-dimensional coordinate system.</font></td>
    </tr>
  </tbody>
</table>