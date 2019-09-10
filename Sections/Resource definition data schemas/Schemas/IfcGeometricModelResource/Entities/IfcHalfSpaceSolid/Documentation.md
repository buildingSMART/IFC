**Definition from ISO/CD 10303-42:1992**: A half space solid is defined by the half space which is the regular subset of the domain which lies on one side of an unbounded surface. The side of the surface which is in the half space is determined by the surface normal and the agreement flag. If the agreement flag is TRUE, then the subset is the one the normal points away from. If the agreement flag is FALSE, then the subset is the one the normal points into. For a valid half space solid the surface shall divide the domain into exactly two subsets. Also, within the domain the surface shall be manifold and all surface normals shall point into the same subset.

> <font size="-1">NOTE A half space is not a subtype of solid model
		  (<i>IfcSolidModel</i>), half space solids are only useful as operands in
		  Boolean expressions.</font>
>

> <font color="#0000FF" size="-1">NOTE Corresponding STEP entity:
		  half_space_solid. Please refer to ISO/IS 10303-42:1994, p. 185 for the final
		  definition of the formal standard. The derived attribute <i>Dim</i> has been
		  added at this level and was therefore demoted from the
		  geometric_representation_item. </font>
> 
> <font color="#0000FF" size="-1">HISTORY New class in IFC Release 1.5
		  </font>
>

**Informal propositions:**

1. The base surface shall divide the domain into exactly two subsets. If the half space solid is of subtype boxed half space (_IfcBoxedHalfSpace_), the domain in question is that of the attribute enclosure. In all other cases the domain is all of space and the base surface shall be unbounded.
2. The base surface shall be an unbounded surface (subtype of _IfcElementarySurface_).

**Illustration**:

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcHalfSpaceSolid-Layout1.dwf"><img src="figures/ifchalfspacesolid-layout1.gif" alt="half space solid" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><font size="-1">Definition of the
			 <i>IfcHalfSpaceSolid</i> within a given coordinate system. The base surface is
			 given by an unbounded plane, the red boundary is shown for visualization
			 purposes only.</font></td> 
		</tr> 
	 </table>