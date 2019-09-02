The following constraints apply to the 'Clipping' representation:

* **Solid**: see standard geometric representation
* **Profile**: see standard geometric representation
* **Extrusion**: see standard geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or subtypes).

Figure 1 illustrates a clipping for a straight wall using an _IfcPolygonalBoundedHalfSpace_ as _SecondOperand_ in the _IfcBooleanClippingResult_.

Figure 2 illustrates a clipping for a curved wall using an _IfcHalfSpaceSolid_ as _SecondOperand_ in the _IfcBooleanClippingResult_.

<table cellpadding="2" cellspacing="2">
<tr>
<td><img src="../../../figures/ifcwallstandard_straigthwall_03-layout1.gif" alt="straight wall clipping" border="0" height="299" width="397"></td>
<td><img src="../../../figures/ifcwallstandard_curvedwall_03-layout1.gif" alt="curved wall clipping" border="0" height="300" width="400"></td>
</tr>
<tr>
<td width="397"><p class="figure">Figure 1 &mdash; Wall body clipping straight</p></td>
<td width="400"><p class="figure">Figure 2 &mdash; Wall body clipping curved</p></td>
</tr>
</table>