The _IfcBSplineCurveForm_ represents a part of a curve of some sppecific form.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> This type is used to indicate that the B-spline curve represents a part of a curve of some specific form.

> NOTE&nbsp; Type adapted from **b_spline_curve_form** defined in ISO 10303-42.

> HISTORY&nbsp; New type in IFC2x2.

{ .spec-head}
Enumerated Item Definitions:

* **polyline form**: A connected sequence of line segments represented by degree 1 B-spline basis functions.
* **circular arc**: An arc of a circle, or a complete circle represented by a B-spline curve.
* **elliptic arc**: An arc of an ellipse, or a complete ellipse, represented by a B-spline curve.
* **parabolic arc**: An arc of finite length of a parabola represented by a B-spline curve.
* **hyperbolic arc**: An arc of finite length of one branch of a hyperbola represented by a B-spline curve.
* **unspecified**: A B-spline curve for which no particular form is specified.