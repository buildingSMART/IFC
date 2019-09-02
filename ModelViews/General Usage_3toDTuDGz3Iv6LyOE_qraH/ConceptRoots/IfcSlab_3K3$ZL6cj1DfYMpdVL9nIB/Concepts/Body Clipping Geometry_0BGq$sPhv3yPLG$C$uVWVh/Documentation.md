The following constraints apply to the 'Clipping' representation:

* **Solid**: see 'SweptSolid' shape representation,
* **Profile**: see 'SweptSolid' shape representation,
* **Extrusion**: see 'SweptSolid' shape representation,
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_.

Figure 1 illustrates a 'Clipping' geometric representation with definition of a roof slab using advanced geometric representation. The profile is extruded non-perpendicular and the slab body is clipped at the eave.

!["advanced slab"](../../../figures/ifcslab_advanced-layout1.gif "Figure 1 &mdash; Slab body clipping")