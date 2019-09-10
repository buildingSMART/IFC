**Definition from ISO/CD 10303-42:1992**: A box domain is an orthogonal box parallel to the axes of the geometric coordinate system which may be used to limit the domain of a half space solid. A box domain is specified by the coordinates of the bottom left corner, and the lengths of the sides measured in the directions of the coordinate axes.

Every semantic object having a physical extent might have a minimum default representation of a bounding box. The bounding box is therefore also used as minimal geometric representation for any geometrically represented object. Therefore the _IfcBoundingBox_ is subtyped from _IfcGeometricRepresentationItem_.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity :
		  box_domain, please refer to ISO/IS 10303-42:1994, p. 186 for the final
		  definition of the formal standard. In IFC the bounding box can also be used
		  outside of the context of an <i>IfcBoxedHalfSpace</i>.</font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 1.0
		  .</font>
>

**Illustration:**

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcBoundingBox-Layout1.dwf"><img src="figures/ifcboundingbox-layout1.gif" alt="half space solid" width="400" height="300" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><font size="-1">The <i>IfcBoundingBox</i>
			 is defined with an own location which can be used to place the
			 <i>IfcBoundingBox</i> relative to the geometric coordinate system. The
			 <i>IfcBoundingBox</i> is defined by the lower left corner (<i>Corner</i>) and
			 the upper right corner (<i>XDim, YDim, ZDim</i> measured within the parent
			 co-ordinate system).</font><font size="-1"></font></td> 
		</tr> 
	 </table>
