A revolved area solid (_IfcRevolvedAreaSolid_) is a solid created by revolving a planar bounded surface about an axis. Both, the axis and planar bounded surface shall be in the same plane and the axis shall not intersect the interior of the swept area. If the swept area has inner boundaries, i.e. holes defined, then those holes shall be swept into holes of the solid. The direction of revolution is clockwise when viewed along the axis in the positive direction.

> <font size="-1">NOTE: The <i>IfcRevolvedAreaSolid</i> now directly
		  defines the revolution of a cross section (also referred to as profile). It
		  thereby combines the functionality of the previous IfcAttDrivenRevolvedSegment
		  entity. In contrary to the previous IfcAttDrivenRevolvedSegment, the additional
		  start angle attribute has been omitted. The axis is required to lie in the xy
		  plane of the position coordinate system.</font>
>

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  revolved_area_solid. Please refer to ISO/IS 10303-42:1994, p. 184 for the final
		  definition of the formal standard. The data type of the inherited
		  <i>SweptArea</i> attribute is different, i.e. of type <i>IfcProfileDef</i>. The
		  position attribute has been added to position the cross section used for the
		  revolution. </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.5, capabilities of this entity have been enhanced in IFC Release 2x.
		  </font>
> 


**Informal propositions:**

1. The _AxisLine_ shall lie in the plane of the _SweptArea_ (as defined at supertype _IfcSweptAreaSolid_).
2. The _AxisLine_ shall not intersect the interior of the _SweptArea_ (as defined at supertype _IfcSweptAreaSolid_).
3. The _Angle_ shall be between 0&deg; and 360&deg;, or 0 and 2<font face="Symbol">p</font> (depending on the unit type for _IfcPlaneAngleMeasure_).

**Illustration**:

<table cellpadding="2" cellspacing="2" border="0"> 
		<tr> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcRevolvedAreaSolid-Layout1.dwf"><img src="figures/ifcrevolvedareasolid-layout1.gif" alt="revolved area solid" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"> 
			 <p><font size="-1"><u>Purpose</u><br>The revolved area solid defines
				the revolution of a 2D area (given by a profile definition) by an axis and
				angle. The result is a solid.</font></p> 
			 <p><font size="-1"><u>Parameter</u><br>The swept area is given by a
				profile definition. This profile is defined </font></p> 
			 <ul> 
				<li><font size="-1">as a 2D bounded curve within the xy plane of
				  the position coordinate system, </font></li> 
				<li><font size="-1">as a 2D bounded curve with holes within the xy
				  plane of the position coordinate system, </font></li> 
				<li><font size="-1">or as a 2D primitive, defined within a 2D
				  position coordinate system, that is placed relative to the xy plane of the
				  position coordinate system</font></li> 
			 </ul></td> 
		</tr> 
	 </table>