**Definition from ISO/CD 10303-46:1992**: An annotation curve occurrence is a curve with a style assignment.

> <font color="#0000ff"><small>
NOTE
&nbsp;Corresponding STEP name:
annotation_curve_occurrence. Please refer to ISO/IS 10303-46:1994 for
the final definition of the formal standard.</small> </font>

&nbsp;The _IfcAnnotationCurveOccurrence_ shall only be used within a material or paper space dependent representation (note: paper space is not yet supported within this IFC release).&nbsp;Styled curves within model space shall use _IfcStyledItem_ as the instance to link the geometric curve&nbsp;representation item to the (shared) style information.

An _IfcAnnotationCurveOccurrence_ is a relation object, that assigns a (set of) styles to a representation item. It can be used without having a geometric representation item already assigned, e.g. within an _IfcMaterialDefinitionRepresentation_. If it has a geometric representation item already assigned than this is further restricted to be a subtype of _IfcCurve_. The applicable style information is restricted to be an _IfcCurveStyle_. For each instance of a styled curve, one instance of _IfcAnnotationCurveOccurrence_&nbsp;has to be created, that points, via an _IfcPresentationStyleAssignment_, to an _IfcCurveStyle_, that can be shared by many styled curves.

> <small><font color="#0000ff">HISTORY
&nbsp;New entity in
Release IFC2x Edition 2.</font></small>