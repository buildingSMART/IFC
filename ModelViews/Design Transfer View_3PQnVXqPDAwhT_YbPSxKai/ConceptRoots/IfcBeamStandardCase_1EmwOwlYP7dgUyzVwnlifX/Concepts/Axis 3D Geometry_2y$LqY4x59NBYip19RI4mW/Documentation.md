The following additional constraints apply to the 'Axis' representation, if the 'Body' shape representation has the _RepresentationType_ : 'SweptSolid':

* _Axis_ 
    * _IfcPolyline_ having two _Points_, or _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcLine_ for 'SweptSolid' provided as _IfcExtrudedAreaSolid_. The axis curve lies on the z axis of the object coordinate system.
    * _IfcTrimmedCurve_ with _BasisCurve_ of Type _IfcCircle_ for 'SweptSolid' provided as _IfcRevolvedAreaSolid_. The axis curve lies on the x/z plane of the object coordinate system, the tangent at the start is along the positive z-axis. 

&nbsp;

<table border="0" cellpadding="2" cellspacing="2" summary="Axis">

<tr><td align="left" valign="top" width="350">
<img src="../../../figures/ifcbeamstandardcase_axis-01.png" alt="Axis" height="300" width="400" border="1"></td>
<td><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 76, the axis shall be defined along the z axis of the object coordinate system. The axis representation can be used to represent the system length of a beam that may extent the body length of the beam.</blockquote>

</td>
</tr>

<tr><td><p class="figure">Figure 1 &mdash; Beam axis representation</p></td><td>&nbsp;</td></tr>

</table>

<table>

<tr><td align="left" valign="top" width="350">
<img src="../../../figures/ifcbeamstandardcase_axis-02.png" alt="Axis" height="300" width="400" border="1"></td>
<td><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 77, the axis representation shall be used to represent the cardinal point as the offset between the 'Axis' and the extrusion path of the beam. The extrusion path is provided as <em>IfcExtrudedAreaSolid.ExtrudedDirection</em> and should be parallel to the 'Axis' and the z axis. It has to be guaranteed that the value provided by
<em>IfcMaterialProfileSetUsage.CardinalPoint</em> is consistent to the <em>IfcExtrudedAreaSolid.Position</em>.</blockquote>

</td>
</tr>

<tr><td><p class="figure">Figure 2 &mdash; Beam axis cardinal point</p></td><td>&nbsp;</td></tr>

</table>