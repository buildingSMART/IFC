The _IfcWindow_, as any subtype of _IfcBuildingElement_, may participate alternatively in one of the two different containment relationships:

* the _Spatial Containment_ (defined here), or
* the _Element Composition_.

The _IfcWindow_ may also be connected to the _IfcOpeningElement_ in which it is placed as a filler. In this case, the spatial containment relationship shall be provided, see Figure 1.

<table>
 
<tr valign="bottom">
  <td><img src="../../../figures/ifcwindow_containment-01.png" alt="Containment" width="600" height="550" border="0"></td>
  <td>
   <blockquote class="note">NOTE&nbsp; The containment shall be defined independently of the filling relationship, that is, even if the 
    <em>IfcWindow</em> is a filling of an opening established by <em>IfcRelFillsElement</em>, it is also contained in the spatial structure 
    by an <em>IfcRelContainedInSpatialStructure</em>.</blockquote>
  </td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Window spatial containment</p></td>
  <td>&nbsp;</td>
 </tr>

</table>