Abstract supertype for the special types defining the object coordinate system. The _IfcObjectPlacement_ has to be provided for each product that has a shape representation.

The object placement can be given:

* absolute, i.e. by an axis2 placement, relative to the world coordinate system,
* relative, i.e. by an axis2 placement, relative to the object placement of another product,
* by grid reference, i.e. by the virtual intersection and reference direction given by two axes of a design grid.

In any case the object placement has to unambiguously define the object coordinate system as either two-dimensional axis placement (_IfcAxis2Placement2D_) or three-dimensional axis placement (_IfcAxis2Placement3D_). The axis placement may have to be calculated.

Informal proposition

1. No two or more elements (subtypes of _IfcProduct_) shall share the same instance of _IfcObjectPlacement_.&nbsp;

> <font color="#0000ff" size="-1">HISTORY
New entity in IFC Release 2x.</font>
>
