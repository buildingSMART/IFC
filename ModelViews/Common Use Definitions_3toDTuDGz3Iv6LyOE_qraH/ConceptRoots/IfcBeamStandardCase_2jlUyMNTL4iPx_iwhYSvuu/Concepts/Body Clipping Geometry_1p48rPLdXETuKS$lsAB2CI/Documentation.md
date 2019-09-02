The following constraints apply to the 'Clipping' representation:

* **Solid** : see 'SweptSolid' geometric representation
* **Solid Position** : see 'SweptSolid' geometric representation
* **Profile** : see 'SweptSolid' geometric representation
* **Profile Position** : see 'SweptSolid' geometric representation
* **Extrusion** : see 'SweptSolid' geometric representation
* **Orientation** : see 'SweptSolid' geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or its subtypes).

Figure 1 illustrates a 'Clipping' geometric representation with use of _IfcBooleanClippingResult_ between an _IfcExtrudedAreaSolid_ and an _IfcHalfSpaceSolid_ to create a clipped body, with cardinal point applied as **4** (mid-depth left)

!["clipped beam"](../../../figures/IfcBeamStandardCase_Clipping-01.png "Figure 1 &mdash; Beam body clipping")