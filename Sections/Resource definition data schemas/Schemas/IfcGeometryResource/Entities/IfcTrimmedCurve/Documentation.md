**Definition from ISO/CD 10303-42:1992**: A trimmed curve is a bounded curve which is created by taking a selected portion, between two identified points, of the associated basis curve. The basis curve itself is unaltered and more than one trimmed curve may reference the same basis curve. Trimming points for the curve may be identified by:

*  parametric value 
* geometric position 
* both of the above 

At least one of these shall be specified at each end of the curve. The _SenseAgreement_ makes it possible to unambiguously define any segment of a closed curve such as a circle. The combinations of sense and ordered end points make it possible to define four distinct directed segments connecting two different points on a circle or other closed curve. For this purpose cyclic properties of the parameter range are assumed; for example, 370 degrees is equivalent to 10 degrees.

The _IfcTrimmedCurve_ has a parameterization which is inherited from the particular basis curve reference. More precisely the parameter s of the trimmed curve is derived from the parameter of the basis curve as follows:

* if _SenseAgreement_ is TRUE: _s = t - t~1~_
*  if _SenseAgreement_ is FALSE: _s = t~2~ - t_ 

In the above equations t~1~ is the value given by _Trim1_ or the parameter value corresponding to point 1 and t~2~ is the value given by _Trim2_ or the parameter value corresponding to point 2. The resultant _IfcTrimmedCurve_ has a parameter ranging from 0 at the first trimming point to |t~2~ - t~1~| at the second trimming point.

> <font size="-1">NOTE In case
of a closed curve,
it may be necessary to increment t1 or t2 by the parametric length for
consistency with the sense flag.</font>
> 


> <font color="#0000ff" size="-1">NOTE
Corresponding STEP entity: trimmed_curve; As a further IFC restriction,
an <i>IfcTrimmedCurve</i> should only trim a <i>IfcLine</i>
or <i>IfcConic</i>. Please refer to ISO/IS 10303-42:1994,
p. 54 for the final definition of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY
New class in IFC Release 1.0 </font>
> 


**Informal Propositions**:

<ol> <li>Where both the parameter value and the Cartesian
point
exist for <i>Trim1</i> and <i>Trim2</i> they
shall be consistent. (i.e., the <i>BasisCurve</i>
evaluated at the parameter value shall coincide with the specified
point).</li> <li>When a Cartesian point is specified by <i>Trim1</i>
or by <i>Trim2</i> it shall lie on the <i>BasisCurve</i>.</li>
<li>Except the case of a closed <i>BasisCurve</i>
where both parameter 1 and parameter 2 exist, they shall be consistent
with the sense flag, i.e., (sense = parameter 1 &lt; parameter 2). <font color="#0000ff">Or, for every open curve where both
parameter 1 and parameter 2 exist, they shall be consistent with the <i>SenseAgreement</i>,
i.e., <i>SenseAgreement</i> = (parameter 1 &lt;
parameter 2).</font></li> <li>If both parameter 1
and parameter 2 exist, then parameter 1
&lt;&gt; parameter 2. <font color="#0000ff">For a
closed base curve, e.g. <i>IfcCircle</i> or <i>IfcEllipse</i>,
this also applies to the cyclic properties, as 360' is equal to 0',
parameter 1 = 360' and parameter 2 = 0' are treated as being equal and
therefore violating this proposition.</font></li> <li>When
a parameter value is specified by <i>Trim1</i>
or <i>Trim2</i> it shall lie within the parametric range
of the <i>BasisCurve</i>.</li>
</ol>
**Additional illustration from IAI:**

!["curve parameterization"](../../../../../../figures/ifctrimmedcurve_parameterization.png "The figure above shows the four arcs (dashed blue and green lines with arrow showing different orientations) that can be defined by the same _BasisCurve_ (of type _IfcCircle_) and the same trimming points (given by Cartesian points and parameter values) by using different assignments to _Trim1_ and _Trim2_ and _SenseAgreement_. <font color="#0000ff"><br> <br>
Note: Since the <i>BasisCurve</i> is closed (type <i>IfcCircle</i>),
the exception of the informal proposition IP3 applies, i.e. the sense
flag is not
required to be consistent with the parameter values of <i>Trim1</i>
and <i>Trim1</i>, so the rule (sense = parameter 1
&lt; parameter 2) may not be fulfilled.</font>")
