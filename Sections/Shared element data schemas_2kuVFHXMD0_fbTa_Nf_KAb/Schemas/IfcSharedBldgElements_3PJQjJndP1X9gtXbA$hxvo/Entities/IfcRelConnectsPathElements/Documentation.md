The _IfcRelConnectsPathElements_ relationship provides the connectivity information between two elements, which have a path information. Currently it is applied to _IfcWall_ and _IfcWallStandardCase_.

The objectified relationship provides all additional information required to describe the connection between two path based elements that might have single or multiple layers of material. The connection type specifies where at the path based element a connection is given (at the start, in the middle or at the end).

> <font size="-1" color="#0000FF">HISTORY: New entity in IFC Release
		  1.5.</font>
>

**Illustration**:

The following figure shows the application of _IfcRelConnectsPathElements_ with the _ConnectionGeometry_ of type _IfcConnectionCurveGeometry_.

<table cellpadding="2" cellspacing="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcRelConnectsPathElements-Layout1.dwf"><img src="figures/IfcRelConnectsPathElements-Layout1.gif" alt="wall connection" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"> 
			 <p><font size="-1">The example shows the connection relationship
				between two instances of <i>IfcWallStandardCase</i> using the
				<i>IfcRelConnectsPathElements</i> relationship. </font></p> 
			 <p><font size="-1">The <i>ConnectionGeometry</i> defines the
				CurveOnRelatingElement and CurveOnRelatedElement, both are of type
				<i>IfcPolyline</i>.</font></p></td> 
		</tr> 
	 </table>