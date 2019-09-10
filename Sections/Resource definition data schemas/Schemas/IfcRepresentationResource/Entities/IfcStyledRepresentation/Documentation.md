**Definition
from IAI**: The _IfcStyledRepresentation_ represents the concept of a styled presentation being a representation of a product or a product component, like material. within a representation context. This representation context does not need to be (but may be) a geometric representation context.

> <small>NOTE&nbsp;
Current usage of <i>IfcStyledRepresentation</i>
includes the assignment of presentation information to an material. The
  <i>IfcStyledRepresentation</i>
then includes presentation styles (<i>IfcAnnotationCurveOccurrence</i>,
  <i>IfcAnnotationFillAreaOccurrence</i>,
  <i>IfcAnnotationSurfaceOccurrence</i>)
that define that a material should be shown within a particular
(eventually view and scale dependent) representation context. All
instances of </small><small><i>IfcStyledRepresentation</i></small><small>
are referenced by <i>IfcMaterialDefinitionRepresentation</i>,
and assigned to <i>IfcMaterial</i>
by </small><small><i>IfcMaterialDefinitionRepresentation.RepresentedMaterial</i>.</small>
> 


A styled representation has to include one or several styled items or annotation occurrences with the associated style information (curve, symbol, text, fill area, or surface styles). It may also contain the geometric representation items that are styled.

> <font color="#0000ff" size="-1">HISTORY: New entity
in
Release IFC 2x Edition 2.</font><font color="#ff0000" size="-1"><br>
  </font>