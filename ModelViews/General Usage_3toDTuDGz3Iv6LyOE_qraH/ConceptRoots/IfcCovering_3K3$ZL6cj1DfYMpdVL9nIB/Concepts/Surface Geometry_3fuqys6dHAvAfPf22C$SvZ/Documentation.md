The following additional constraints apply to the 'GeometricSet' representation of _IfcCovering_:

* for planar base surfaces - bounded surface representation
* for cylindrical base surfaces - swept surface representation

&nbsp;

<table>

 <tr>

  <td><img src="../../../figures/ifccovering_standard-1-layout1.gif" alt="standard planar covering" border="0" height="274" width="399"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates a planar surface representation where the
area of <em>IfcCovering</em> is given by an <em>IfcPolyLoop</em> for
planar base surfaces (here provided by the
<em>IfcRelSpaceBoundary</em>). The implicit planar surface of the <em>IfcPolyLoop</em> shall be
identical with the planar surface defined by the
<em>IfcRelSpaceBoundary</em>.</blockquote></td>
 </tr>

 <tr>

  <td>
<p class="figure">Figure 1 &mdash; Covering surface planar</p>
</td>

 </tr>

</table>

<table>

 <tr>

  <td><img src="../../../figures/ifccovering_standard-2-layout1.gif" alt="standard cylindrical covering" border="0" height="274" width="399"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates a cylindrical surface representation where
the area of the <em>IfcCovering</em> is given by an
<em>IfcSurfaceOfLinearExtrusion</em> for cylindrical base surfaces
(here given by the <em>IfcRelSpaceBoundary</em>, such as caused by a
round wall).</blockquote>
  <blockquote>

   <ul>
    
<li class="small">The geometry representation of the <em>IfcCovering</em> is given
by the <em>IfcTrimmedCurved</em> (the Curve parameter of the
<em>IfcArbitraryOpenProfileDef</em> - in cases of faceted
representation also an <em>IfcPolyline</em>). It is extruded within
the plane of the base surface using the <em>Depth</em> parameter of
the <em>IfcSurfaceOfLinearExtrusion</em>.</li>
</ul></blockquote>
</td>
 
</tr>
 
<tr>

  <td>
<p class="figure">Figure 2 &mdash; Covering surface
cylindrical</p>
</td>
  <td>&nbsp;</td>

</tr>

</table>