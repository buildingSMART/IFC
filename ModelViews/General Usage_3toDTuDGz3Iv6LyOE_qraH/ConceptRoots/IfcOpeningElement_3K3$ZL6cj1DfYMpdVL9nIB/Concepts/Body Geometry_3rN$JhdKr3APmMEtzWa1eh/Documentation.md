Currently, the 'Body', and 'Box' representations are supported. The 'Box' representation includes the representation type 'BoundingBox' and is explained at _IfcFeatureElement_.

The 'Body' representation of _IfcOpeningElement_ can be represented using the representation types 'SweptSolid', and 'Brep'. The representation type 'Brep' is explained at _IfcFeatureElement_

_Swept Solid Representation Type with Horizontal
Extrusion_

The 'SweptSolid' geometric representation of _IfcOpeningElement_, using horizontal extrusion direction (for walls), is defined using the swept area solid geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required, the set of _IfcShapeRepresentation.Items_ may include a single, or multiple, instances of _IfcExtrudedAreaSolid_.
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded horizontally (perpendicular to the extrusion direction of the voided element such as for wall openings), or vertically (in the extrusion direction of the voided element such as for for floor openings). If multiple instances of _IfcExtrudedAreaSolid_ are used, the extrusion direction of each extrusion should be equal.

> NOTE&nbsp; In case of non-parallel jambs, the shape representation shall be a 'SweptSolid' representation with vertical extrusion.

Figure 1 illustrates an opening with horizontal extrusion.

> NOTE&nbsp; The local placement directions for the _IfcOpeningElement_ are only given as an example, other directions are valid as well.

!["standard opening"](../../../figures/ifcopeningelement_horizontal-layout1.png "Figure 1 &mdash; Opening with full extrusion")

Figure 2 illustrates an opening for a recess.

> NOTE&nbsp; The local placement directions for the _IfcOpeningElement_ are only given as an example, other directions are valid as well.

> NOTE&nbsp; Rectangles are now defined centric, the placement location has to be set:

* _IfcCartesianPoint_(XDim/2,YDim/2)

!["recess"](../../../figures/ifcopeningelement_recess-layout1.png "Figure 2 &mdash; Opening with recess extrusion")

_Swept Solid Representation with Vertical Extrusion_

The 'SweptSolid' geometric representation of _IfcOpeningElement_, using vertical extrusion direction (for walls), is defined using the swept area solid geometry, however the extrusion direction may be vertical, i.e. in case of a wall opening, the extrusion would be in the direction of the wall height. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required, the set of _IfcShapeRepresentation.Items_ may include a single, or multiple, instances of _IfcExtrudedAreaSolid_.
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded vertically, i.e. for wall openings along the extrusion direction of the voided element.  If multiple instances of _IfcExtrudedAreaSolid_ are used, the extrusion direction should be equal.

Vertical extrusions shall be used when an opening or recess has a non rectangular foot print geometry that does not change along the height of the opening or recess.

Figure 3 shows a vertical extrusion with multiple extrusion bodies for the opening. Each extrusion body has a different extrusion lenght.

> NOTE&nbsp; The local placement directions for the _IfcOpeningElement_ are only given as an example, other directions are valid as well.

!["vertical extrusion"](../../../figures/ifcopeningelement_vertical-layout1.png "Figure 3 &mdash; Opening with multiple extrusions")