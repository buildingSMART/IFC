The following constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcRectangleProfileDef, IfcCircleProfileDef , IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.

Figure 1 illustrates a 'SweptSolid' geometric representation.

> NOTE&nbsp; The following interpretation of dimension parameter applies for polygonal slabs (in ground floor view): > * _IfcArbitraryClosedProfileDef.OuterCurve_: closed bounded curve interpreted as area (or foot print) of the slab.

!["standard slab"](../../../figures/ifcslab_standard-layout1.gif "Figure 1 &mdash; Slab body extrusion")

The following additional constraints apply to the 'SweptSolid' representation, when an _IfcMaterialLayerSetUsage_ is assigned to the _IfcSlab_:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_, _IfcRectangleProfileDef_, _IfcCircleProfileDef_, _IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.
* **Material**: The definition of the _IfcMaterialLayerSetUsage_, particularly of the _OffsetFromReferenceLine_ and the _ForLayerSet.TotalThickness_, has to be consistent to the 'SweptSolid' representation.

&nbsp;

<table>
 
<tr>
  <td><img src="../../../figures/ifcslab_standard-layout1.gif" alt="standard slab" border="0" height="274" width="399"></td>
  <td>

<blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates a 'SweptSolid' geometric representation. The following interpretation of dimension parameter applies for polygonal slabs (in ground floor view):
 <em>IfcArbitraryClosedProfileDef.OuterCurve</em>: closed bounded curve interpreted as area (or foot print) of the slab.</blockquote>

</td>
 </tr>

 <tr>
  <td><p class="figure">Figure 2 &mdash; Slab body extrusion</p></td>
  <td>&nbsp;</td>
 </tr>

</table>