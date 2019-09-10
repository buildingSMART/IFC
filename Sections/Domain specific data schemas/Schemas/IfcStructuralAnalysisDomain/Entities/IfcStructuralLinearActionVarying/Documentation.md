Instances of the entity _IfcStructuralLinearActionVarying_ are used to define varying linear actions. _IfcStructuralLinearActionVarying_ inherits the needed attributes and applicable structural load types from its superclass _IfcStructuralLinearAction_.

> <font size="-1">NOTE: This entity definition inherits from its
		  superclass <i>IfcStructuralActivity</i> the mandatory attribute
		  <i>AppliedLoad</i>. It is used as the first list member of the derived list
		  <i>VaryingAppliedLoads</i></font>
> 


> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
> 


****Topology Use Definition****

Instances of _IfcStructuralLinearActionVarying_ shall have a topology representation. It includes a placement and a product representation. The _IfcProductRepresentation_ shall be given by an item of _Representations_ being of type "_IfcTopologyRepresentation_". The definition of the topological representation is given at the supertype _IfcStructuralLinearAction_. One additional constraint applies:

* The topology representation has to be given by an _IfcEdgeCurve_ to provide a parameterized geometric representation of the curve between both vertices. This parameterization is needed for the location of the varying loads.

****Shape Aspect Use Definition****

The attribute _VaryingAppliedLoadLocation_ reference a shape aspect, that has a list of _ShapeRepresentations_. Each individual _IfcShapeRepresentation_ within that list shall have a single item within its list of _Items_. The type of the item shall be either:

* _IfcCartesianPoint_, or
* _IfcPointOnCurve_

Each list member within the list of _ShapeRepresentations_ corresponds to the list member (at same position) of the list _VaryingAppliedLoads_, and provides the position of the applied load. At least two applied load values shall be given, the distribution of the applied linear loads across the surface of the planar action is constructed by linear interpolation.

The following examples shows a definition of a varying applied loads by four points on curve.

<table cellspacing="2" cellpadding="2" border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1"><b>VaryingAppliedLoads<br>Position</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>VaryingAppliedLoads<br>Value</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>VaryingThicknessLocation</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>Point on curve</b></font></td> 
		  <td valign="TOP"><font size="-1"><b>Parameter value</b></font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[1]</font><br><font size="-1">identical with <i>AppliedLoad</i></font></td> 
		  <td valign="TOP"><font size="-1">8</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.
			 ShapeRepresentations[1]</font></td> 
		  <td valign="TOP"><font size="-1">Items[1]<br>TYPEOF
			 IfcPointOnCurve</font></td> 
		  <td valign="TOP"><font size="-1">0.</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[2]</font></td> 
		  <td valign="TOP"><font size="-1">8</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.
			 ShapeRepresentations[2]</font></td> 
		  <td valign="TOP"><font size="-1">Items[2]<br>TYPEOF
			 IfcPointOnCurve</font></td> 
		  <td valign="TOP"><font size="-1">0.35</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[3]</font></td> 
		  <td valign="TOP"><font size="-1">12</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.
			 ShapeRepresentations[3]</font></td> 
		  <td valign="TOP"><font size="-1">Items[3]<br>TYPEOF
			 IfcPointOnCurve</font></td> 
		  <td valign="TOP"><font size="-1">0.35</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[4]</font></td> 
		  <td valign="TOP"><font size="-1">12</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.
			 ShapeRepresentations[4]</font></td> 
		  <td valign="TOP"><font size="-1">Items[4]<br>TYPEOF
			 IfcPointOnCurve</font></td> 
		  <td valign="TOP"><font size="-1">0.65</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP"><font size="-1">[5]</font></td> 
		  <td valign="TOP"><font size="-1">0</font></td> 
		  <td valign="TOP"><font size="-1">IfcShapeAspect.ShapeRepresentations[5]</font></td> 
		  <td valign="TOP"><font size="-1">Items[4]<br>TYPEOF
			 IfcPointOnCurve</font></td> 
		  <td valign="TOP"><font size="-1">0.85</font></td> 
		</tr> 
	 </table>

**Example:**

!["linear action varying"](../../../../../../figures/ifcstructurallinearactionvarying-fig1.gif "&nbsp;<font size="-1">Example for the definition of a varying
				linear action. </font>")