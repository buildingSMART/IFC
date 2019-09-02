The wall axis is represented by a two-dimensional open curve within a particular shape representation. The 'Axis' shape representation is only used to locate the material layer set along the axis, if the _IfcMaterialLayerSetUsgae_ is applied to the _IfcWall_. In this case, the wall axis is used to apply the material layer set usage parameter to the wall geometry.

* _Axis_ 
    * _IfcPolyline_ having two _Points_, or _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcLine_ for the 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the x/y plane and is parallel to the x-axis of the object coordinate system.
    * _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcCircle_ for 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the x/y plane of the object coordinate system, the tangent at the start is along the positive x-axis. 

&nbsp;

<table cellpadding="2" cellspacing="2">

 <tr>

  <td align="left" valign="top"><img src="../../../figures/ifcwallstandard_straigthwall_01-layout1.gif" alt="straight wall axis" border="0" height="299" width="393"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates an axis representation for a straight wall. In case of a straight wall, the set of items shall
include a single geometric representation item of type <em>IfcPolyline</em> or <em>IfcTrimmedCurve</em> with the <em>BasisCurve</em> being an <em>IfcLine</em>. The <em>IfcPolyline</em> or <em>IfcTrimmedCurve</em> shall be parallel (here in a special case co-linear) to the x-axis
of the object coordinate system. The direction shall be identical to the direction of the x-axis.</blockquote>

 </td>
 </tr>
 <tr>
  <td width="393"><p class="figure">Figure 1 &mdash; Wall axis straight</p></td>

  <td>&nbsp;</td>
 </tr>
</table>

<table cellpadding="2" cellspacing="2">

 <tr>

  <td align="left" valign="top"><img src="../../../figures/ifcwallstandard_curvedwall_01-layout1.gif" alt="curved wall axis" border="0" height="299" width="393"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates an axis representation for a curved wall. In case of a curved wall, the set of items shall include
a single geometric representation item of type <em>IfcTrimmedCurve</em>. The curve shall have a <em>BasisCurve</em> of type <em>IfcCircle</em>. The tangent of the <em>IfcTrimmedCurve</em> shall be parallel at start to the x-axis of the object coordinate system. The direction shall be identical to the direction of the x-axis.</blockquote>
 </td></tr>
 
<tr>
  <td width="393"><p class="figure">Figure 2 &mdash; Wall axis curved</p></td>
  <td>&nbsp;</td>
 
</tr>

</table>