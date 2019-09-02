A rational Bezier curve is a B-spline curve described in terms of control points and basic functions. It describes weights in addition to the control points defined at the supertype _IfcBSplineCurve_.

> <font size="-1">NOTE: The <i>IfcRationalBezierCurve</i> is an entity
		  that had been adopted from ISO 10303, Industrial automation systems and
		  integration&#151;Product data representation and exchange, Part 42: Integrated
		  generic resource: Geometric and topological
		  representation.</font>
>

> <font size="-1">NOTE: The specific subtype
		  <i>IfcRationalBezierCurve</i> has been introduced to avoid the complexity of
		  ANDOR subtype relationships in the ISO 10303-42
		  specification</font>
>

All weights shall be positive and the curve is given by:

![Math](figures/IfcRationalBezierCurve-Math1.gif)where

<table> 
		<tr> 
		  <td width="100" align="RIGHT"><i>k</i>+1</td> 
		  <td>number of control points</td> 
		</tr> 
		<tr> 
		  <td align="RIGHT">P<sub><i>i</i></sub></td> 
		  <td>control points</td> 
		</tr> 
		<tr> 
		  <td align="RIGHT"><i>w<sub>i</sub></i></td> 
		  <td>weights</td> 
		</tr> 
		<tr> 
		  <td align="RIGHT"><i>d</i></td> 
		  <td>degree</td> 
		</tr> 
	 </table>

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  rational_b_spline_curve. Please refer to ISO/IS 10303-42:1994, p. 45 for the
		  final definition of the formal standard. </font>
> 
> <font size="-1" color="#0000FF">HISTORY: New entity in Release IFC2x
		  Edition 2.</font>
>