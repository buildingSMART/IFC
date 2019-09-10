**Definition
from IAI**:&nbsp;The _IfcAnnotationSurfaceOccurrence_ shall only be used within a material or paper space dependent representation (note: paper space is not yet supported within this IFC release).&nbsp;Styled surfaces or solids within model space shall use _IfcStyledItem_ as the instance to link the geometric surface, solid or annotation surface (for texture maps) representation item to the (shared) style information.

An _IfcAnnotationSurfaceOccurrence_ is a relation object, that assigns a (set of) styles to a representation item. It can be used without having a geometric representation item already assigned, e.g. within an _IfcMaterialDefinitionRepresentation_. Each instance of _IfcAnnotationSurfaceOccurrence_&nbsp;points, via an _IfcPresentationStyleAssignment_, to an _IfcSurfaceStyle_, that can be shared by many styled surfaces, or solids.

> <font color="#0000ff"><small>NOTE&nbsp;
No direct
corresponding STEP
entity, the entity has been defined in analogy to the other annotation
occurrence entity.</small> </font>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in
Release IFC2x Edition 2.</font><font color="#ff0000"><br>
  </font></small>