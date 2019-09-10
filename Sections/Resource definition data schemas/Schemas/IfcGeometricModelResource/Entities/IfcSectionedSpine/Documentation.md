**Definition from ISO/DIS 10303-42-ed2:1999**: A sectioned spine is a representation of the shape of a three dimensional object composed of a spine curve and a number of planar cross sections. The shape is defined between the first element of cross sections and the last element of this set.

> NOTE A sectioned spine may be used to represent a surface or a solid but the interpolation of the shape between the cross-sections is not defined. For the representation of a solid all cross-sections are closed curves.
>

A sectioned spine (_IfcSectionedSpine_) is a representation of the shape of a three dimensional object composed by a number of planar cross sections, and a spine curve. The shape is defined between the first element of cross sections and the last element of the cross sections. A sectioned spine may be used to represent a surface or a solid but the interpolation of the shape between the cross sections is not defined.

For the representation of a solid all cross sections are areas. For representation of a surface all cross sections are curves. The cross sections are defined as profiles, whereas the consecutive profiles may be derived by a transformation of the start profile or the previous consecutive profile.

The spine curve shall be of type _IfcCompositeCurve_, each of its segments (_IfcCompositeCurveSegment_) shall correspond to the part between exactly two consecutive cross-sections.

> <font size="-1">NOTE: The <i>IfcSectionedSpine</i> combines the
		  functionality of the previous entities IfcAttDrivenTaperedExtrudedSegment,
		  IfcAttDrivenMorphedExtrudedSegment, IfcAttDrivenTaperedRevolvedSegment,
		  IfcAttDrivenMorphedRevolvedSegment.</font>
>

> <font color="#0000FF" size="-1"><font color="#0000FF" size="-1">NOTE:
		  Corresponding STEP entity: sectioned spine. Please refer to ISO/DIS
		  10303-42-ed2:1999, p. 282 for the definition of the formal standard. The cross
		  sections are defined in IFC as <i>IfcProfileDef</i>. The position coordinate
		  systems are added.</font></font>
> 
> <font color="#0000FF" size="-1">HISTORY New entity in IFC Release 2x.
		  </font>
>

<table cellpadding="2" cellspacing="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcSectionedSpine-Layout1.dwf"><img src="figures/ifcsectionedspine-layout1.gif" alt="spine 1" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"> 
			 <p>Example of an <i>IfcSectionedSpine</i></p> 
			 <ul> 
				<li><font size="-1">The <i>SpineCurve</i> is given by an
				  <i>IfcCompositeCurve</i> with two <i>Segments</i>. The <i>Segments[1]</i> has a
				  <i>ParentCurve</i> of type <i>IfcPolyline</i> and a <i>Transition</i> =
				  CONTSAMEGRADIENT. The <i>Segments[2]</i> has a <i>ParentCurve</i> of type
				  <i>IfcTrimmedCurve</i> and a <i>Transition</i> = DISCONTINUOUS.</font></li> 
				<li><font size="-1">Each <i>CrossSectionPosition</i> lies at a
				  start or end point of the <i>Segments</i>.</font></li> 
				<li><font size="-1">Each <i>CrossSections</i> are inserted by the
				  <i>CrossSectionPositions</i>. The first two cross sections are of type
				  <i>IfcRectangleProfileDef</i>, the third is of type
				  <i>IfcDerivedProfileDef</i>.</font></li> 
			 </ul></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcSectionedSpine.wrl"><img src="figures/ifcsectionedspine.jpg" alt="render" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"> 
			 <p><font size="-1">Final result of the <i>IfcSectionedSpine</i>. The
				body (shown transparently) is not fully defined by the exchange
				definition.</font></p></td> 
		</tr> 
	 </table>

**Informal propositions**

1.  non of the cross sections, after being placed by the cross section positions, shall intersect 
2. non of the cross sections, after being placed by the cross section positions, shall lie in the same plane
3. the local origin of each cross section position shall lie at the beginning or end of a composite curve segment.