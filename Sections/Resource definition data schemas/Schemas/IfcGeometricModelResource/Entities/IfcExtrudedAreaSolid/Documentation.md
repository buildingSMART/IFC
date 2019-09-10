The extruded area solid (_IfcExtrudedAreaSolid_) is defined by sweeping a bounded planar surface. The direction of the extrusion is given by the _ExtrudedDirection_ attribute and the length of the extrusion is given by the _Depth_ attribute. If the planar area has inner boundaries, i.e. holes defined, then those holes shall be swept into holes of the solid.

> <font size="-1"><u>New</u>: The <i>IfcExtrudedArea</i> solid now
		  directly defines the linear extrusion of a cross section (also referred to as
		  profile). It thereby combines the functionality of the previous
		  IfcAttDrivenExtrudedSegment entity. In contrary to the previous
		  IfcAttDrivenExtrudedSegment, the extruded direction can be any which is not
		  perpendicular to the z axis of the position coordinate
		  system.</font>
>

The _ExtrudedDirection_ is given within the position coordinate system as defined by _IfcSweptAreaSolid.Position_. Extrusions are not longer restricted to be perpendicular to the extruded surface of the profile.

> <font color="#0000FF" size="-1"><font color="#0000FF" size="-1">NOTE
		  Corresponding STEP entity: extruded_area_solid. Please refer to ISO/IS
		  10303-42:1994, p. 183 for the final definition of the formal standard. The data
		  type of the inherited <i>SweptArea</i> attribute is different, i.e. of type
		  <i>IfcProfileDef</i>. The <i>Position</i> attribute has been added to position
		  the cross section used for the linear extrusion.</font></font>
> 
> <font color="#0000FF" size="-1">HISTORY New entity in IFC Release 1.5,
		  capabilities of this entity have been enhanced in IFC Release 2x.
		  </font>
>

**Illustration**:

<table cellpadding="2" cellspacing="2" border="0"> 
		<tr> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcExtrudedAreaSolid-Layout1.dwf"><img src="figures/ifcextrudedareasolid-layout1.gif" alt="extruded area solid" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"> 
			 <p><font size="-1"><u>Purpose</u><br>The extruded area solid defines
				the extrusion of a 2D area (given by a profile definition) by an direction and
				depth. The result is a solid.</font></p> 
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