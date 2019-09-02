The _IfcDoor_, as any subtype of _IfcBuildingElement_, may participate alternatively in one of the two different containment relationships:

* the _Spatial Containment_ (defined here), or
* the _Element Composition_.

The _IfcDoor_ may also be connected to the _IfcOpeningElement_ in which it is placed as a filler. In this case, the spatial containment relationship shall be provided, see Figure 1.

<table>
 
<tr valign="bottom">
  
<td><img src="../../../figures/IfcDoor_Containment-01.png" alt="Containment" width="500" height="460" border="0"></td>
  
<td>
<blockquote class="note">NOTE&nbsp; The containment shall be
defined independently of the filling relationship, that is, even if

   the <em>IfcDoor</em> is a filling of an opening established by
<em>IfcRelFillsElement</em>, it is also contained in the spatial
structure by
   <em>IfcRelContainedInSpatialStructure</em>.</blockquote>
</td>

 </tr>

 <tr>
  
<td>
<p class="figure">Figure 1 &mdash; Door spatial containment</p>
</td>

  <td>&nbsp;</td>
 
</tr>

</table>