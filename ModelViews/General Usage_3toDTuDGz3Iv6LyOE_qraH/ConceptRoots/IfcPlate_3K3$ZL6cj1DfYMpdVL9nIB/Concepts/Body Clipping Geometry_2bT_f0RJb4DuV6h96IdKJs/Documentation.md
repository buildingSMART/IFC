The following constraints apply to the 'Clipping' representation when an _IfcMaterialLayerSetUsage_ is assigned to the _IfcPlate_:

* **Solid**: see 'SweptSolid' shape representation,
* **Profile**:&nbsp;see 'SweptSolid' shape representation,
* **Extrusion**:&nbsp;see 'SweptSolid' shape representation,
* **Material**:&nbsp;see 'SweptSolid' shape representation,
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_.

&nbsp;

<table>

 <tr>
  <td><img src="../../../figures/ifcslab_advanced-layout1.gif" alt="advanced plate" border="0" height="274" width="399"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates a 'Clipping' geometric representation with definition of a plate using advanced geometric representation. The profile is extruded non-perpendicular and the plate body is clipped at the eave.</blockquote>

</td>
 </tr>

 <tr>
  <td><p class="figure">Figure 1 &mdash; Plate body clipping</p></td>
  <td>&nbsp;</td>
 </tr>

</table>