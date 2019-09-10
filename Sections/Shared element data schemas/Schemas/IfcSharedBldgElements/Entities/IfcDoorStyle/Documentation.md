**Definition
from IAI**: The door style, _IfcDoorStyle_, defines a particular style of doors, which may be included into the spatial context of the building model through an (or multiple) instances of _IfcDoor_. A door style defines the overall parameter of the door style and refers to the particular parameter of the lining and one (or several) panels through the _IfcDoorLiningProperties_ and the _IfcDoorPanelProperties_.

The door entity, _IfcDoor_, defines a particular occurrence of a door inserted in the spatial context of a project. The actual parameter of the door and/or its shape is defined at the _IfcDoorStyle_, to which the _IfcDoor_ is related by the inverse relationship _IsDefinedBy_ pointing to _IfcRelDefinedByType_. The _IfcDoorStyle_ also defines the particular attributes for the lining_,
IfcDoorLiningProperties_, and panels, _IfcDoorPanelProperties_.

> <small><font color="#0000ff">HISTORY&nbsp;
New entity
in IFC Release 2x.</font></small>

> <small><font color="#ff0000">IFC2x
Edition 2
COMPATIBILITY NOTICE&nbsp; The entity <i>IfcDoorStyle</i>
is still subtyped from the <i>IfcTypeProduct</i>
to provide upward compatibility. This is a recorded anomaly as all
other types for building elements are now subtyped from <i>IfcBuildingElementType</i>
and have the suffix "Type", not "Style".</font>
  </small>

****Geometry
Use Definitions****:

The _IfcDoorStyle_ defines the baseline geometry, or the representation map, for all occurrences of the door style, given by the _IfcDoor_, pointing to this style. The representation of the door style may be given by the agreed set of minimal parameters, defined for the door lining and the door panel(s), or it may be given by a geometric representation used by the _IfcRepresentationMap_. The attribute _ParameterTakesPrecedence_ decides, whether the set of parameters can be used to exactly represent the shape of the door style (TRUE), or whether the attached _IfcRepresentationMap_ holds the exact representation (FALSE).

**Interpretation
of parameter**

The _IfcDoorStyleOperationTypeEnum_ defines the general layout of the door style. Depending on the enumerator, the appropriate instances of _IfcDoorLiningProperties_ and _IfcDoorPanelProperties_ are attached in the list of _HasPropertySets_. The _IfcDoorStyleOperationTypeEnum_mainly determines the hinge side (left hung, or right hung), the operation (swinging, sliding, folding, etc.)&nbsp;and the number of panels.

See geometry use definitions at _IfcDoorStyleOperationTypeEnum_for the correct usage of opening symbols for different operation types.