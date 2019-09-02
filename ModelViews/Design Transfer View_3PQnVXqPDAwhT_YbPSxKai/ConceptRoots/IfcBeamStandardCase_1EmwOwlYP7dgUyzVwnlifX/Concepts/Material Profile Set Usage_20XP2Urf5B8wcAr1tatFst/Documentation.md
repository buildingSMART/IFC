The _IfcBeamStandardCase_ defines in addition that the _IfcBeamType_ should have a unique _IfcMaterialProfileSet_, that is referenced by the _IfcMaterialProfileSetUsage_ that is assigned to all occurrences of this _IfcBeamType_.

<table>

 <tr>
  <td><img src="../../../figures/ifcbeamstandardcase-01.png" height="500" width="500" alt="Material profile set and usage"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialProfileSetUsage</em> and <em>IfcMaterialProfileSet</em> to the <em>IfcBeamStandardCase</em> as the beam occurrence and to the <em>IfcBeamType</em>. The same <em>IfcMaterialProfileSet</em> shall be shared by many occurrences of <em>IfcMaterialProfileSetUsage</em>. This relationship shall be consistent to the relationship between the <em>IfcBeamType</em> and the <em>IfcBeamStandardCase</em>.</blockquote>

 </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Beam profile usage</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table>

 <tr>
  <td><img src="../../../figures/ifcbeamstandardcase_cardinalpoint.png" width="675" alt="Cardinal point usage"></td>
  <td>

    <blockquote class="example">EXAMPLE&nbsp; Figure 2 illustrates alignment of cardinal points.</blockquote>
    
<blockquote class="note">NOTE&nbsp; It has to be guaranteed that the use of <em>IfcCardinalPointEnum</em> is consistent to the placement of the extrusion body provided by <em>IfcExtrudedAreaSolid.Position</em></blockquote>
    
<blockquote class="note">NOTE&nbsp; The cardinal points <b>8</b> (top centre) and <b>6</b> (mid-depth right) are assigned according to the definition at <em>IfcCardinalPointReference</em></blockquote> </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 2 &mdash; Beam cardinal points</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table>
 
<tr>
  <td><img src="../../../figures/ifcbeamstandardcase-02.png" height="550" width="500" alt="Material profile set and usage"></td>
  <td>
<blockquote class="example">EXAMPLE&nbsp; Figure 3 illustrates assignment of a composite profile by using <em>IfcCompositeProfile</em> for geometric representation and several <em>IfcMaterialProfile</em>'s within the <em>IfcMaterialProfileSet</em>.</blockquote>

 </td>
 </tr>

 <tr>
  <td><p class="figure">Figure 3 &mdash; Beam composite profiles</p></td>
 </tr>

</table>