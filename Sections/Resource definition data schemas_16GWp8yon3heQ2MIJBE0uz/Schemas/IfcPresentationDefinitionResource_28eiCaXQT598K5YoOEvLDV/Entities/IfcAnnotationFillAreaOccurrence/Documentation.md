**Definition
from ISO/CD 10303-46:1992**: An annotation fill area occurrence is a fill area with a style assignment.

> <font color="#0000ff"><small>
NOTE&nbsp;
Corresponding STEP
name: annotation_fill_area_occurrence. Please refer to ISO/IS
10303-46:1994 for the final definition of the formal standard.</small>
  </font>

**Definition
from IAI**:&nbsp;The _IfcAnnotationFillAreaOccurrence_ shall only be used within a material or paper space dependent representation (note: paper space is not yet supported within this IFC release).&nbsp;Styled filled areas within model space shall use _IfcStyledItem_ as the instance to link the geometric filled area representation item to the (shared) style information.

An _IfcAnnotationFillAreaOccurrence_ is a relation object, that assigns a (set of) styles to a representation item. It can be used without having a geometric representation item already assigned, e.g. within an _IfcMaterialDefinitionRepresentation_. If it has a geometric representation item already assigned than this is further restricted to be a subtype of _IfcAnnotationFillArea_. The applicable style information is restricted to be an _IfcFillAreaStyle_.&nbsp;For each instance of a styled fill area, one instance of _IfcAnnotation__FillArea__Occurrence_ has to be created, that points, via an _IfcPresentationStyleAssignment_, to an _Ifc__FillArea__Style_, that can be shared by many styled fill areas.

The _IfcAnnotationFillAreaOccurrence_ determines how an _IfcFillAreaStyle_, and in particular how an included _IfcFillAreaStyleHatching_ or _IfcFillAreaStyleTiles_, is placed at a particular annotation occurrence. The _FillStyleTarget_ specifies the point (if omitted it defaults to the origin) at which the (virtual) point of origin of the hatching style is placed, it can either be:

*  a point relative to the world coordinate system (if _GlobalOrLocal_ = .GLOBAL.), or    
* a point relative to the local (object) coordinate system (if _GlobalOrLocal_ = .LOCAL.), or    
* a point relative to the surface parameterization (if _GlobalOrLocal_ is omitted).   

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in
Release IFC2x Edition 2. </font><br>
  <font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; The <i>IfcAnnotationFillAreaOccurrence</i>
has changed by making the attribute <i>FillStyleTarget</i>
OPTIONAL and by adding the attribute <i>GlobalOrLocal</i>.</font></small>