**Definition from ISO/CD 10303-42:1992**: The location and orientation in two dimensional space of two mutually perpendicular axes. An axis2_placement_2d is defined in terms of a point, (inherited from the placement supertype), and an axis. It can be used to locate and originate an object in two dimensional space and to define a placement coordinate system. The class includes a point which forms the origin of the placement coordinate system. A direction vector is required to complete the definition of the placement coordinate system. The reference direction defines the placement X axis direction, the placement Y axis is derived from this.

If the _RefDirection_ attribute is not given, the placement defaults to P[1] (x-axis) as [1.,0.] and P[2] (y-axis) as [0.,1.].

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP name:
		  axis2_placement_2d, please refer to ISO/IS 10303-42:1994, p. 28 for the final
		  definition of the formal standard. </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.5.</font>
>

**Illustration**

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcAxis2Placement2D-Layout1.dwf"><img src="figures/ifcaxis2placement2d-layout1.gif" alt="axis2 placement 2D" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><font size="-1">Definition of the
			 <i>IfcAxis2Placement2D</i> within the two-dimensional coordinate
			 system.</font></td> 
		</tr> 
	 </table>
