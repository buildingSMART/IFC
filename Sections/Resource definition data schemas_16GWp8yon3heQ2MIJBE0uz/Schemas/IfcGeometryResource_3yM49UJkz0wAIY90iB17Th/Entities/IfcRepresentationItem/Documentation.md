The _IfcRepresentationItem_ is used within an _IfcRepresentation_ (directly or indirectly through other _IfcRepresentationItem_'s) to represent an _IfcProductRepresentation_. Most commonly these _IfcRepresentationItem_'s are geometric or topological representation items, that can (but not need to) have presentation style infomation assigned.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-43:1992  
> A representation item is an element of product data that participates in one or more representations or contributes to the definition of another representation item. A representation item contributes to the definition of another representation item when it is referenced by that representation item.

> NOTE&nbsp; The assignment of a style is only applicable to the subtypes _IfcGeometricRepresentationItem_, _IfcMappedItem_ and some selected subtypes of _IfcTopologicalRepresentationItem_ (_IfcVertexPoint_, _IfcEdgeCurve_, _IfcFaceSurface_).

In case that presentation style information is applied, it can be either applied by an _IfcStyledItem_, or by an assignment to an _IfcPresentationLayerWithStyle_. If both are present, and both style assignments include the same subtype of _IfcPresentationStyle_, then the style assigned by _IfcStyledItem_ takes priority.

Figure 1 shows an instance diagram explaining the use of _IfcStyledItem_ and _IfcPresentationLayerWithStyle_ to apply presentation styles.

> EXAMPLE&nbsp; The assignment of style information by a styled item and a presentation layer with style. Since the presentation styles are different, _IfcCurveStyle_ and _IfcSurfaceStyle_, both are applied to the geometric representation item.

!["styles assigned by layer and styled item"](../../../figures/ifcrepresentationitem_style-1.png "Figure 1 &mdash; Representation item style")

Figure 2 shows in instance diagram explaining the override of _IfcPresentationLayerWithStyle_ by _IfcStyledItem_ to apply presentation styles.

> EXAMPLE&nbsp; The assignment of style information by a styled item and a presentation layer with style. Since the presentation styles for curve style are aprovided by both, the _IfcCurveStyle_ provided by the _IfcStyledItem_ overrides the _IfcCurveStyle_ provided by the _IfcPresentationLayerWithStyle_

!["styles assigned by layer and styled item"](../../../figures/ifcrepresentationitem_style-2.png "Figure 2 &mdash; Representation item style override")

> NOTE&nbsp; Entity adapted from **representation_map** defined in ISO 10303-43.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The inverse attributes _StyledByItem_ and _LayerAssignments_ have been added. Upward compatibility for file based exchange is guaranteed.