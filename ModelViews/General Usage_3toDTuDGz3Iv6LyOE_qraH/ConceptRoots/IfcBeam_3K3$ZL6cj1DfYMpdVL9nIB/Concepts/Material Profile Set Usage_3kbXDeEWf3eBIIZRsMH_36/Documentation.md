The _Material Profile Set Usage_ defines the assignment of an _IfcMaterialProfileSetUsage_ to the _IfcBeamType_ providing a common profile definition to all occurrences of this _IfcBeamType_. Beams with composite profile can be represented by refering to several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ that is referenced from the _IfcMaterialProfileSetUsage_.

<table>

 <tr>
  <td><img src="../../../figures/ifcbeam-01.png" height="500" width="500" alt="Material profile set and usage"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialProfileSetUsage</em> and <em>IfcMaterialProfileSet</em> to the <em>IfcBeam</em> as the beam occurrence and to the <em>IfcBeamType</em>. The same <em>IfcMaterialProfileSet</em> shall be shared by many occurrences of <em>IfcMaterialProfileSetUsage</em>. This relationship shall be consistent to the relationship between the <em>IfcBeamType</em> and the <em>IfcBeam</em>.</blockquote>

 </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Beam profile usage</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

<table>

 <tr>
  <td><img src="../../../figures/ifcbeam_cardinalpoint.png" height="250" width="500" alt="Cardinal point usage"></td>
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
  <td><img src="../../../figures/ifcbeam-02.png" height="550" width="500" alt="Material profile set and usage"></td>
  <td>
<blockquote class="example">EXAMPLE&nbsp; Figure 3 illustrates assignment of a composite profile by using <em>IfcCompositeProfile</em> for geometric representation and several <em>IfcMaterialProfile</em>'s within the <em>IfcMaterialProfileSet</em>.</blockquote>

 </td>
 </tr>

 <tr>
  <td><p class="figure">Figure 3 &mdash; Beam composite profiles</p></td>
 </tr>

</table>