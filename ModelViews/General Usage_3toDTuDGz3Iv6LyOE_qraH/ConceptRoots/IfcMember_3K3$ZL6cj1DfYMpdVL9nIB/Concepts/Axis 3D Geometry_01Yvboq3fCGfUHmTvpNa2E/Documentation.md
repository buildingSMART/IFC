The axis representation can be used to represent the system length of a member that may extent the body length of the member.

> NOTE&nbsp; The 'Axis' is used to locate the material profile set, if the material association is of type _IfcMaterialProfileSetUsage_.

The following additional constraints apply to the 'Axis' representation, if an _IfcMaterialProfileSetUsage_ is provided and the 'Body' shape representation has the _RepresentationType_: 'SweptSolid':

* _Axis_ 
    * _IfcPolyline_ having two _Points_, or _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcLine_ for 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the z axis of the object coordinate system.
    * _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcCircle_ for 'SweptSolid' provided as _IfcRevolvedAreaSolid_. The axis curve lies on the x/z plane of the object coordinate system, the tangent at the start is along the positive z-axis. 

&nbsp;

<table border="0" cellpadding="2" cellspacing="2" summary="Axis">
 
<tr>
  <td align="left" valign="top" width="350"><img src="../../../figures/ifcmemberstandardcase_axis-01.png" alt="Axis" border="1"></td>
  <td>

<blockquote class="example">EXAMPLE&nbsp; As shown in Figure 101, the axis representation can be used to represent the system length of a member that may extent the body length of the member.</blockquote>

 </td>
 </tr>

 <tr>
  <td><p class="figure">Figure 1 &mdash; Member axis representation</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table border="0" cellpadding="2" cellspacing="2" summary="Axis">
 
<tr>
  <td align="left" valign="top" width="350"><img src="../../../figures/ifcmemberstandardcase_axis-02.png" alt="Axis" border="1"></td>
  <td align="left" valign="top"><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 102, the axis representation shall be used to represent the cardinal point as the offset between the 'Axis' and the extrusion path of the member. The extrusion path is provided as <em>IfcExtrudedAreaSolid.ExtrudedDirection</em> and should be parallel to the 'Axis'.  It has to be guaranteed that the value provided by <em>IfcMaterialProfileSetUsage.CardinalPoint</em> is consistent to the <em>IfcExtrudedAreaSolid.Position</em>.</blockquote>

</td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 2 &mdash; Member axis cardinal point</p></td>
  <td>&nbsp;</td>
 </tr>

</table>