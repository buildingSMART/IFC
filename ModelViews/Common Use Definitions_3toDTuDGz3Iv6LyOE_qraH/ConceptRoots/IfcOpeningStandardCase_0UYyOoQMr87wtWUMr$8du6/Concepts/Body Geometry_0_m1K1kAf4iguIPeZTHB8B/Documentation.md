The geometric representation of _IfcOpeningStandardCase_ is defined using the following multiple shape representations for its definition:

* Body: A SweptSolid representation defining the 3D subtraction shape of the standard opening

**Body Representation**

The body representation of _IfcOpeningStandardCase_ is represented using the representation type 'SweptSolid'.

_Swept Solid Representation Type with Horizontal
Extrusion_

The standard geometric representation of _IfcOpeningStandardCase_ is defined using the 'SweptSolid' representation. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used::

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: a single _IfcExtrudedAreaSolid_ is required
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded horizontally (i.e. perpendicular to the extrusion direction of the voided element) for wall openings, or vertically (i.e. in the extrusion direction of the voided element), for slab openings.

As shown in Figure 36, the orientation of the opening profile that is extruded for the opening body shall guarantee the following interpretation of dimension parameter for rectangular openings:

* _IfcRectangleProfileDef.YDim_ interpreted as opening width
* _IfcRectangleProfileDef.XDim_ interpreted as opening height

!["standard opening"](../../../figures/IfcOpeningStandardCase_Wall-Layout1.png "Figure 1 &mdash; Opening standard representation")