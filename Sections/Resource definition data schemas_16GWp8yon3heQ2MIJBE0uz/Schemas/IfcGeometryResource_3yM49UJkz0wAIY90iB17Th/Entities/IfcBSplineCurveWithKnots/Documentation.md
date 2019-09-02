The _IfcBSplineCurveWithKnots_ is a spline curve parameterized by spline functions for which the knot values are explicitly given.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> This is the type of b-spline curve for which the knot values are explicitly given. This subtype shall be used to represent non-uniform B-spline curves and may be used for other knot types.  
> Let _L_ denote the number of distinct values amongst the _d_+_k_+2 knots in the knot list; _L_ will be referred to as the &lsquo;upper index on knots&rsquo;. Let _m~j~_ denote the multiplicity (i.e., number of repetitions) of the _j_th distinct knot. Then:  
>   
> ![formula](../../../figures/ifcbsplinecurve-math2.gif)  
>   
> All knot multiplicities except the first and the last shall be in the range 1,...,_d_; the first and last may have a maximum value of _d_ + 1. In evaluating the basis functions, a knot _u_ of, e.g., multiplicity 3 is interpreted as a sequence _u_, _u_, _u_,; in the knot array.

> NOTE&nbsp; Entity adapted from **b_spline_curve_with_knots** defined in ISO10303-42.

> HISTORY&nbsp; New entity in IFC4.