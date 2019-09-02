Instances of the entity _IfcStructuralSurfaceMemberVarying_ shall be used to describe planar structural elements with a varying thickness.

The inherited _Thickness_ attribute shall be given, the additional, subsequent thickness values are given by the _SubsequentThickness_ list. The derived list _VaryingThickness_ is created by pushing the_Thickness_ attribute at the beginning of the _SubsequentThickness_ list.

> <font size="-1">NOTE: The list <i>VaryingThickness</i> and the list
		  <i>ShapeRepresentations</i> of the referenced <i>IfcShapeAspect</i> are
		  corresponding lists.</font>
>

> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
> 


****Topology Use Definition****

Instances of _IfcStructuralSurfaceMemberVarying_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_". The guidelines on using the location and topological representation capabilities are identical with those at the supertype _IfcStructuralSurfaceMember_.

****Shape Aspect Use Definition****

The attribute _VaryingThicknessLocation_ references a shape aspect that has a list of _ShapeRepresentations_. Each individual _IfcShapeRepresentation_ within that list shall have a single item within its list of _Items_. The type of the item shall be either:

* _IfcCartesianPoint_, or
* _IfcPointOnSurface_

Each list member within the list of _ShapeRepresentations_ corresponds to the list member (at same position) of the list _VaryingThickness_, and provides the thickness at that location. At least three thickness values shall be given, the analytical volume is constructed by triangulation.

The following example shows a definition of a varying thickness by four Cartesian points.

<table cellspacing="4" cellpadding="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1"><b>VaryingThickness<br>Position</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>VaryingThickness<br>Value</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>VaryingThicknessLocation</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>Point</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>Coordinates</b></font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[1]</font></td> 
		  <td valign="TOP"><font size="-1">0.2</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.ShapeRepresentations[1]</font></td> 
		  <td valign="TOP"><font size="-1">Items[1]<br>TYPEOF
			 IfcCartesianPoint</font></td> 
		  <td valign="TOP"><font size="-1">[0.,0.]</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[2]</font></td> 
		  <td valign="TOP"><font size="-1">0.3</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.ShapeRepresentations[2]</font></td> 
		  <td valign="TOP"><font size="-1">Items[2]<br>TYPEOF
			 IfcCartesianPoint</font></td> 
		  <td valign="TOP"><font size="-1">[1.,0.]</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[3]</font></td> 
		  <td valign="TOP"><font size="-1">0.4</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.ShapeRepresentations[3]</font></td> 
		  <td valign="TOP"><font size="-1">Items[3]<br>TYPEOF
			 IfcCartesianPoint</font></td> 
		  <td valign="TOP"><font size="-1">[1.,1.]</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[4]</font></td> 
		  <td valign="TOP"><font size="-1">0.3</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.ShapeRepresentations[4]</font></td> 
		  <td valign="TOP"><font size="-1">Items[4]<br>TYPEOF
			 IfcCartesianPoint</font></td> 
		  <td valign="TOP"><font size="-1">[0.,1.]</font></td> 
		</tr> 
	 </table>

> <font size="-1">NOTE: The units for the Value and the coordinates of
		  the Cartesian point are given at the global unit assignment by<i>
		  IfcProject.UnitsInContext</i>. In the example meter is
		  used.</font>
>