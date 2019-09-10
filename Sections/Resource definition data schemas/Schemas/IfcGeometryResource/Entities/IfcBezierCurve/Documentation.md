**Definition from ISO/CD 10303-42:1992**: This is a special type of curve which can be represented as a type of B-spline curve in which the knots are evenly spaced and have high multiplicities. Suitable default values for the knots and knot multiplicities are derived in this case.

A B-spline curve is _a piecewise Bezier_ curve if it is quasi-uniform except that the interior knots have multiplicity _degree_ rather than having multiplicity one. In this subtype the knot spacing is 1.0, starting at 0.0. A _piecewise Bezier_ curve which has only two knots, 0.0 and 1.0, each of multiplicity (degree+1), is a simple Bezier curve.

> <font size="-1">NOTE: A simple Bezier curve can be defined as a
		  B-spline curve with knots by the following data: </font>
>

<table> 
		<tr> 
		  <td width="100">&nbsp;</td> 
		  <td width="200"><font size="-1">degree</font></td> 
		  <td><font size="-1"> (d)</font></td> 
		</tr> 
		<tr> 
		  <td>&nbsp;</td> 
		  <td><font size="-1">upper index on control points</font></td> 
		  <td><font size="-1">(equal to d) </font></td> 
		</tr> 
		<tr> 
		  <td>&nbsp;</td> 
		  <td><font size="-1">control points</font></td> 
		  <td><font size="-1"> (d + 1 cartesian points) </font></td> 
		</tr> 
		<tr> 
		  <td>&nbsp;</td> 
		  <td><font size="-1">knot type</font></td> 
		  <td><font size="-1"> (equal to quasi-uniform knots)</font></td> 
		</tr> 
	 </table>

> <font size="-1">No other data are needed, except for a rational Bezier
		  curve. In this case the weights data ((d + 1) REALs) shall be given.
		  </font>
>

> <font size="-1">NOTE: It should be noted that every piecewise Bezier
		  curve has an equivalent representation as a B-spline curve but not every
		  B-spline curve can be represented as a Bezier curve. </font>
>

> <font size="-1">To define a<i> piecewise Bezier</i> curve as a
		  B-spline:</font>
>

> <ul> 
		  <li><font size="-1">The first knot is 0.0 with multiplicity (d + 1).
			 </font></li> 
		  <li><font size="-1">The next knot is 1.0 with multiplicity d (we have
			 now defined the knots for one segment, unless it is the last one). </font></li>
		  
		  <li><font size="-1">The next knot is 2.0 with multiplicity d (we have
			 now defined the knots for one segment, again unless the second is the last
			 one). </font></li> 
		  <li><font size="-1">Continue to the end of the last segment, call it
			 the n-th segment, at the end of which a knot with value n, multiplicity (d + 1)
			 is added.</font></li> 
		</ul>

> <font size="-1">EXAMPLE:</font>
>

> <ul> 
		  <li><font size="-1">A one-segment cubic Bezier curve would have knot
			 sequence (0,1) with multiplicity sequence (4,4). </font></li> 
		  <li><font size="-1">A two-segment cubic <i>piecewise Bezier</i> curve
			 would have knot sequence (0,1,2) with multiplicity sequence (4,3,4).
			 </font></li> 
		</ul>

> <font size="-1">For the<i> piecewise Bezier</i> case, if <i>d</i> is
		  the degree, <i>m</i> is the number of knots with multiplicity <i>d</i>, and
		  <i>N</i> is the total number of knots for the spline,
		  then</font>
>

<table> 
		<tr> 
		  <td width="100">&nbsp;</td> 
		  <td width="200" align="RIGHT"><font size="-1">(d+2+k)&nbsp;</font></td>
		  
		  <td><font size="-1">&nbsp;= N</font></td> 
		</tr> 
		<tr> 
		  <td>&nbsp;</td> 
		  <td align="RIGHT"><font size="-1">&nbsp;</font></td> 
		  <td><font size="-1">&nbsp;= (d+1)+md+(d+1)</font></td> 
		</tr> 
		<tr> 
		  <td>&nbsp;</td> 
		  <td align="RIGHT"><font size="-1">thus m&nbsp;</font></td> 
		  <td><font size="-1">&nbsp;= (k-d)/d </font></td> 
		</tr> 
	 </table>

> <font size="-1">So the knot sequence is (0; 1; ...;<i>m</i>;
		  (<i>m</i>+ 1)) with multiplicities (<i>d</i> + 1; <i>d</i>; : : :; <i>d</i>;
		  <i>d</i>+ 1).</font>
>

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  bezier_curve. Please refer to ISO/IS 10303-42:1994, p. 51 for the final
		  definition of the formal standard. Due to the constraints in the IFC
		  architecture to not include ANDOR subtype constraints, an explicit subtype
		  IfcRationalBezierCurve is added which holds the same information as the complex
		  entity b_spline_curve AND bezier_curve.</font>
> 
> <font size="-1" color="#0000FF">HISTORY: New entity in Release IFC2x
		  Edition 2.</font>
>
