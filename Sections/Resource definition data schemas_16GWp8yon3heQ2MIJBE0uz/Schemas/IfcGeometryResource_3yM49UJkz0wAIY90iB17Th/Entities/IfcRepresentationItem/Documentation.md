**Definition
from ISO/CD 10303-43:1992**: A representation item is an element of product data that participates in one or more representations or contributes to the definition of another representation item. A representation item contributes to the definition of another representation item when it is referenced by that representation item.

**Definition
from IAI**&nbsp; The _IfcRepresentationItem_ is used within (and only within - directly or indirectly through other _IfcRepresentationItem_'s or _IfcShapeAspect_'s) an _IfcRepresentation_ to represent an _IfcProductRepresentation_. Most commonly these _IfcRepresentationItem_'s are geometric or topological representation items, that can (but not need to) have presentation style infomation assigned.

> <small>NOTE&nbsp;
Corresponding
STEP entity: representation_item. Please refer to ISO/IS 10303-43:1994,
for the final definition of the formal standard. The following changes
have been made: The attribute 'name' and the WR1 have not been
incorporated.</small>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 2x.</font></small>  
> <small><font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp;
The inverse attributes <i>StyledByItem</i>
and <span style="font-style: italic;">LayerAssignments</span>
have been added.
Upward compatibility for file based exchange is guaranteed.</font></small>