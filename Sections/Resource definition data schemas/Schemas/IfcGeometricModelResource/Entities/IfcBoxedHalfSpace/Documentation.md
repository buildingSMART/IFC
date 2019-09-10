**Definition from ISO/CD 10303-42:1992**: This entity is a subtype of the half space solid which is trimmed by a surrounding rectangular box. The box has its edges parallel to the coordinate axes of the geometric coordinate system.

> <font size="-1">NOTE: The purpose of the box is to facilitate CSG
		  computations by producing a solid of finite size.</font>
>

The _IfcBoxedHalfSpace_ (from ISO 10303-42:1994 boxed_half_space) is used (as its supertype _IfcHalfSpaceSolid_) only within Boolean operations. It divides the domain into exactly two subsets, where the domain in question is that of the attribute _Enclosure_.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity :
		  boxed_half_space, please refer to ISO/IS 10303-42:1994, p. 185 for the final
		  definition of the formal standard. The IFC class <i>IfcBoundingBox</i> is used
		  for the definition of the enclosure, providing the same definition as
		  box_domain. </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.5.1, improved documentation available in IFC Release
		  2x.</font>
>

**Illustration:**

<table frame="BORDER" width="100%"> 
		<tr> 
		  <td width="420" valign="TOP" align="LEFT"><a href="drawings/IfcBoxedHalfSpace-Layout1.dwf"><img src="figures/ifcboxedhalfspace-layout1.gif" border="0" height="300" width="400"></a></td> 
		  <td align="LEFT" valign="TOP" width="100%"> 
			 <p><font size="-1"><u>Purpose</u> <br>The <i>IfcBoundingBox</i>
				(relating to ISO 10303-42:1994 box_domain) that provides the enclosure is given
				for the convenience of the receiving application to enable the use of size box
				comparison for efficiency (e.g., to check first whether size boxes intersect,
				if not no calculations has to be done to check whether the solids of the
				entities intersect).</font></p> 
			 <p><font size="-1"><u>Parameter</u> <br>The <i>Enclosure</i>
				therefore helps to prevent dealing with infinite-size related issues. The
				enclosure box is positioned within the positioning coordinate system of the
				unbounded surface, given by the attribute <i>BaseSurface</i> (see
				<i>IfcElementarySurface.Position</i>). The <i>AgreementFlag</i> defines whether
				the box is defined into the direction of the positive z axis (FALSE) or in the
				direction of the negative z axis (TRUE).</font></p></td> 
		</tr> 
	 </table>