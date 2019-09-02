The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcArbitraryProfileDefWithVoids, IfcRectangleProfileDef, IfcCircleProfileDef, IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.

The following additional constraints apply to the 'SweptSolid' representation, when an _IfcMaterialLayerSetUsage_ is assigned to the _IfcPlate_:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcRectangleProfileDef, IfcRoundedRectangleProfileDef, IfcCircleProfileDef, IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.
* **Material**: The definition of the _IfcMaterialLayerSetUsage_, particularly of the _OffsetFromReferenceLine_ and the _ForLayerSet.TotalThickness_, has to be consistent to the 'SweptSolid' representation.

&nbsp;

<table>

 <tr>
  <td><img src="../../../figures/ifcslab_standard-layout1.gif" alt="standard plate" border="0" height="274" width="399"></td>
  <td>

<blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates a 'SweptSolid' geometric representation. The following interpretation of dimension parameter applies for polygonal plates (in ground floor view): <em>IfcArbitraryClosedProfileDef.OuterCurve</em> being a closed bounded curve is interpreted as area (or foot print) of the plate.</blockquote>


 </td>
 </tr>

 <tr>
  <td><p class="figure">Figure 1 &mdash; Plate body extrusion</p></td>
  <td>&nbsp;</td>
 </tr>

</table>