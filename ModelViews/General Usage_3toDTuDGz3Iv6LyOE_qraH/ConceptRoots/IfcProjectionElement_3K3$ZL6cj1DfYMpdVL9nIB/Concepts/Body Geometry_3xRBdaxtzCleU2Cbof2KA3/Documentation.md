The geometric representation of _IfcProjectionElement_ is defined using the swept area solid geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required.
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded horizontally (that is, perpendicular to the extrusion direction of the modified element), such as for wall projections, or vertically (that is, in the extrusion direction of the projected element), such as for floor projections.

As shown in Figure 1, the following interpretation of dimension parameter applies for rectangular projection:

* _IfcRectangleProfileDef.YDim_ interpreted as projection width
* _IfcRectangleProfileDef.XDim_ interpreted as projection height
* _IfcExtrudedAreaSolid.Depth_ is interpreted as projection depth

> NOTE&nbsp; Rectangles are now defined centric, the placement location has to be set: > * _IfcCartesianPoint_(XDim/2,YDim/2)

> NOTE&nbsp; The local placement directions for the _IfcProjectionElement_ are only given as an example, other directions are valid as well.

!["projection"](../../../figures/ifcprojectionelement-layout1.png "Figure 1 &mdash; Projection representation")

The general b-rep geometric representation of _IfcProjectionElement_ is defined using the Brep geometry. The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'Brep'