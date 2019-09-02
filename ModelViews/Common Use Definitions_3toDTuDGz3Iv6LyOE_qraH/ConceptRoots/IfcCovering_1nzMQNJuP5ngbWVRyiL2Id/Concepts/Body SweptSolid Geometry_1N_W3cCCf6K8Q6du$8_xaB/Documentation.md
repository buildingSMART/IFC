The following additional constraints apply to the 'SweptSolid' representation of _IfcCovering_:

* for planar base surfaces - swept area representation
* for cylindrical base surfaces - swept area representation

&nbsp;

<table>
 
<tr>
  
<td><img src="../../../figures/IfcCovering_Advanced-1-Layout1.gif" alt="advanded solid covering" border="0" height="274" width="399"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates a body representation where the volume of
<em>IfcCovering</em> is given by an <em>IfcExtrudedAreaSolid</em> for
planar base surfaces (here given by the
<em>IfcRelSpaceBoundary</em>). The extruded area (<em>IfcArbitraryClosedProfileDef</em>) shall 
be coplanar to the surface defined by the
<em>IfcRelSpaceBoundary</em>.
</blockquote></td>
 </tr>

 <tr>
  
<td>
<p class="figure">Figure 1 &mdash; Covering body planar</p>
</td>

  <td>&nbsp;</td>
 </tr>

</table>

<table>
 
<tr>
  
<td><img src="../../../figures/IfcCovering_Advanced-2-Layout1.gif" alt="advanced solid covering" border="0" height="274" width="399"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates a body representation where the volume of
the <em>IfcCovering</em> is given by an <em>IfcExtrudedAreaSolid</em>
for cylindrical base surfaces (here given by the
<em>IfcRelSpaceBoundary</em> - such as caused by a round wall).</blockquote>
  <blockquote>
   
<ul>
<li class="small">The geometry representation of the <em>IfcCovering</em> is given
by the <em>IfcCompositeCurve</em> (the <em>OuterCurve</em> parameter of
the <em>IfcArbitraryClosedProfileDef</em> - in cases of faceted
representation also a closed <em>IfcPolyline</em>). It is extruded
along the plane of the base surface using the <em>Depth</em>
parameter of the <em>IfcSurfaceOfLinearExtrusion</em>.</li>
</ul></blockquote>
 </td>
 </tr>
 
<tr>
  
<td>
<p class="figure">Figure 2 &mdash; Covering body circular</p>
</td>

  <td>&nbsp;</td>
 </tr>

</table>