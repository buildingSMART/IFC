**Definition
from ISO/CD 10303-46:1992**: An annotation text occurrence is a text with a style assignment.

> <font color="#0000ff"><small>
NOTE&nbsp;
Corresponding
STEP name: annotation_text_occurrence. Please refer to ISO/IS
10303-46:1994 for the final definition of the formal standard.</small>
  </font>

&nbsp;The _IfcAnnotationTextOccurrence_shall only be used within a material or paper space dependent representation (note: paper space is not yet supported within this IFC release).&nbsp;Styled text within model space shall use _IfcStyledItem_ as the instance to link the geometric text representation item to the (shared) style information.

An _IfcAnnotationTextOccurrence_is a relation object, that assigns a (set of) styles to a representation item. It can be used without having a geometric representation item already assigned, e.g. within an _IfcMaterialDefinitionRepresentation_. If it has a geometric representation item already assigned than this is further restricted to be&nbsp;an _IfcTextLiteral__. The applicable style information is restricted to be an&nbsp;_IfcTextStyle._&nbsp;For each instance of a styled text, one instance of _IfcAnnotationTextOccurrence_ has to be created, that points, via an _IfcPresentationStyleAssignment_, to an _IfcTextStyle_, that can be shared by many styled texts.

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in Release IFC2x Edition 2.</font></small>