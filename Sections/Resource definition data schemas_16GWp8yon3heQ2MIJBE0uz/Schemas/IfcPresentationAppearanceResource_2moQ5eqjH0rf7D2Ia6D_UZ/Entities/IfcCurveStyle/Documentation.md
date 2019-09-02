**Definition
from ISO/CD 10303-46:1992**: A curve style specifies the visual appearance of curves.

An _IfcCurveStyle_ provides the style table for presentation information assigned to geometric curves. The style is defined by a color, a font and a width. <font color="#0000ff">The <i>IfcCurveStyle&nbsp;</i>defines
curve patterns as model patterns, i.e. the distance between visible and
invisible segments of
curve patterns are given in model space dimensions (that
have to be scaled using the target plot scale). </font>

Styles are intended to be shared by multiple _IfcStyledItem_'s, assigning the style to occurrences of (subtypes of) _IfcGeometricRepresentationItem_'s. Measures given to a font pattern or a curve width are given in global drawing length units.

> <small>NOTE&nbsp;
global units are defined at the single <i>IfcProject</i>
instance, given by <i>UnitsInContext:IfcUnitAssignment</i>,
the same
units are used for the geometric representation items and for the style
definitions.</small>
> 


The measure values for font pattern and curve width <font color="#0000ff">apply to
the
model space </font>with a target plot scale provided for the correct appearance in the default plot scale.. For different scale and projection dependent curve styles a different instance of _IfcCurveStyle_ needs to be used by _IfcPresentationStyleAssignment_ for different _IfcGeometricRepresentationSubContext_ dependent representations.

> <small>NOTE&nbsp;
the target plot scale is given by <i>IfcGeometricRepresentationSubContext.TargetScale</i>.</small>  
>

An _IfcCurveStyle_ can be assigned to _IfcGeometricRepresentationItem_'s via the _IfcPresentationStyleAssignment_ through an intermediate _IfcStyledItem_ or _IfcAnnotationCurveOccurrence_.

> <font color="#0000ff"><small>NOTE&nbsp;
Corresponding
STEP name:
curve_style. Please refer to ISO/IS 10303-46:1994 for the final
definition of the formal standard.</small> </font>

> <font color="#0000ff"><small>HISTORY&nbsp;
New entity in
Release IFC2x Edition 2.</small> </font>