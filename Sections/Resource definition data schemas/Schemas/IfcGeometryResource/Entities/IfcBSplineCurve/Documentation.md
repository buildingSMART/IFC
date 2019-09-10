**Definition from ISO/CD 10303-42:1992**: A B-spline curve is a piecewise parametric polynomial or rational curve described in terms of control points and basis functions. The B-spline curve has been selected as the most stable format to represent all types of polynomial or rational parametric curves. With appropriate attribute values it is capable of representing single span or spline curves of explicit polynomial, rational, Bezier or B-spline type.

Interpretation of the data is as follows:

<ol> 
		<li> 
		  <p>All weights shall be positive and the curve is given by</p><img src="figures/ifcbsplinecurve-math1.gif" width="183" height="115" border="0"> 
		  <table> 
			 <tr> 
				<td align="RIGHT" width="100"><i>k</i>+1</td> 
				<td> = number of control points</td> 
			 </tr> 
			 <tr> 
				<td align="RIGHT" width="100">P<sub><i>i</i></sub></td> 
				<td>= control points</td> 
			 </tr> 
			 <tr> 
				<td align="RIGHT" width="100"><i>w</i><sub><i>i</i></sub></td> 
				<td>= weights</td> 
			 </tr> 
			 <tr> 
				<td align="RIGHT" width="100"><i>d</i></td> 
				<td>= degree</td> 
			 </tr> 
		  </table> 
		  <p>The knot array is an array of (<i>k</i>+<i>d</i>+2) real numbers
			 [<i>u</i><sub>-<i>d</i></sub> ... <i>u</i><sub><i>k</i>+1</sub>], such that for
			 all indices j in [-<i>d</i>,<i>k</i>], <i>u</i><sub>j</sub> &lt;=
			 <i>u</i><sub>j+1</sub>. This array is obtained from the knot data list by
			 repeating each multiple knot according to the multiplicity. <i>N
			 <sup>d</sup><sub>i</sub></i>, the <i>i</i>th normalized B-spline basis function
			 of degree <i>d</i>, is defined on the subset [<i>u<sub>i-d</sub></i>, ... ,
			 <i>u<sub>i+1</sub></i>] of this array.</p></li> 
		<li> 
		  <p>Let <i>L</i> denote the number of distinct values among the
			 <i>d</i>+<i>k</i>+2 knots in the knot array; <i>L</i> will be referred to as
			 the 'upper index on knots'. Let <i>m<sub>j</sub></i> denote the multiplicity
			 (i.e. number of repetitions) of the <i>j</i>th distinct knot. Then</p>
		  <img src="figures/ifcbsplinecurve-math2.gif" width="149" height="59" border="0"> 
		  <p>All knot multiplicities except the first and the last shall be in
			 the range 1 ... degree; the first and last may have a maximum value of degree +
			 1. In evaluating the basis functions, a knot <i>u</i> of e.g. multiplicity 3 is
			 interpreted as a string <i>u, u, u,</i> in the knot array. The B-spline curve
			 has 3 special subtypes (<i>IAI note: only 1, Bezier curve, included in this IFC
			 release</i>) where the knots and knot multiplicities are derived to provide
			 simple default capabilities.</p></li> 
		<li>Logical flag is provided to indicate whether the curve self
		  intersects or not.</li> 
	 </ol>
**Illustration from ISO 10303-42**:

![control points](../../../../../../figures/ifcbsplinecurve-fig1.gif)
> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  b_spline_curve. Please refer to ISO/IS 10303-42:1994, p. 45 for the final
		  definition of the formal standard. </font>
> 
> <font size="-1" color="#0000FF">HISTORY: New entity in Release IFC2x
		  Edition 2.</font>
>
