An _IfcCompositeCurve_ is a continuous curve composed of curve segments.

Figure 1 illustrates an example of a composite curve.

!["formula"](../../../figures/ifccompositecurve.png "Figure 1 &mdash; Composite curve")

Consider an _IfcCompositeCurve_ having line segment and an arc segment. The line should be parameterized:

* _IfcPolyline_ with start= 0.,0. end= 0.,1., _SameSense_= TRUE, parametric length = 1.

The arch should be parameterized:

* _IfcTrimmedCurve_ with start= 180', end= 90', _SameSense_= FALSE, parametric length = 90.

Then the parameterization of the composite curve is:

* _IfcCompositeCurve_ with 0. &le; T &le; 1. (line segment) and 1. &le; T &le; 91. (arc segment), parametric length = 91.

&nbsp;

{ .extDef}
> NOTE Definition according to ISO 10303-42:  
> A composite curve is a collection of curves joined end-to-end. The individual segments of the curve are themselves defined as composite curve segments. The parameterization of the composite curve is an accumulation of the parametric ranges of the referenced bounded curves. The first segment is parameterized from _0_ to _l~<small>1</small>~_ and for _i__&le;__2_, the _i^<small>th</small>^_ segment is parameterized from:
> 
>> ![formula](../../../figures/ifccompositecurve-math1.gif)
> where _l~<small>k</small>~_ is the parametric length (i.e., difference between maximum and minimum parameter values) of the curve underlying the _k^<small>th</small>^_ segment. Let _T_ denote the parameter for the composite curve. Then, if the _i_th segment is not a reparameterised composite curve segment, _T_ is related to the parameter _t~i~_; _t~i0~__&le;__t~i~__&le;__t~i1~_; for the _i_th segment by the equation:
> 
>> ![formula](../../../figures/ifccompositecurve-math2.gif) if _Segments[i].SameSense_ = TRUE;
> or by the equation:
> 
>> ![formula](../../../figures/ifccompositecurve-math3.gif) if _Segments[i].SameSense_ = FALSE;
> If the segments[i] is of type reparameterised composite curve segment,
> 
>> ![formula](../../../figures/ifccompositecurve-math4.gif) where _&tau;_ is defined at reparameterized composite curve segment (see _IfcReparameterizedCompositeCurveSegment_).


> 
> NOTE&nbsp; Entity adapted from **composite_curve** defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC1.0

{ .spec-head}
Informal Propositions:

1. The _SameSense_ attribute of each segment correctly specifies the senses of the component curves. When traversed in the direction indicated by _SameSense_, the segments shall join end-to-end.