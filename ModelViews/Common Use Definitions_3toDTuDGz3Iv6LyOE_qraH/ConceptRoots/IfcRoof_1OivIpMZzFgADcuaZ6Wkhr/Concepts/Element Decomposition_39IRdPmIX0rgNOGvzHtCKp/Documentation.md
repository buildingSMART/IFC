_Geometric representation by aggregated elements_

If the _IfcRoof_ has components (referenced by _SELF\IfcObject.IsDecomposedBy_) then no independent geometric representation shall defined for the _IfcRoof_. The _IfcRoof_ is then geometrically represented by the geometric representation of its components. The components are accessed via _SELF\IfcObject.IsDecomposedBy[1].RelatedObjects_. The geometric representations that are supported for the aggregated elements are defined with each element. See geometric use definition for _IfcSlab_, _IfcBeam_, _IfcColumn_, _IfcBuildingElementPart_ and other subtypes of _IfcBuildingElement_.

Figure 1 illustrates roof placement, with an _IfcRoof_ defining the local placement for all aggregated elements.

!["roof"](../../../figures/IfcRoof-Layout1.gif "Figure 1 &mdash; Roof placement")