The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ is required.
* **Extrusion**: All extrusion directions shall be supported.

The following additional constraints apply to the 'SweptSolid' representation, when an _IfcMaterialLayerSetUsage_ is assigned to the _IfcSlab_:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ and _IfcRectangleProfileDef_ shall be supported.
* **Extrusion**: The profile shall be extruded vertically, i.e., in the direction of the z-axis of the co-ordinate system of the referred spatial structure element. It might be further constraint to be in the direction of the global z-axis in implementers agreements. The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the Position of the _IfcExtrudedAreaSolid_.

The profile of a wall is described in the ground view and extruded vertically. The profile (also identical with the foot print of the wall) is defined by the _IfcArbitraryClosedProfileDef_ (excluding its subtypes). The profile is given with all wall connections already resolved.

Figure 1 illustrates a body representation for a straight wall. In case of a straight wall, the two sides of the profile shall be parallel to the wall axis, that is, the wall has a single unchanged thickness.

Figure 2 illustrates a body representation for a curved wall. In case of a curved wall, the two sides of the profile shall be parallel (with defined offset) to the wall axis, that is, the wall has a single unchanged thickness.

<table cellpadding="2" cellspacing="2">
 
<tr>

  <td align="left" valign="top"><img src="../../../figures/ifcwallstandard_straigthwall_02-layout1.gif" alt="straight wall body" border="0" height="299" width="393"></td>

  <td align="left" valign="top"><img src="../../../figures/ifcwallstandard_curvedwall_02-layout1.gif" alt="curved wall body" border="0" height="299" width="393"></td>

 </tr>

 <tr>
  
<td width="393"><p class="figure">Figure 1 &mdash; Wall body extrusion straight</p></td>

  <td width="393"><p class="figure">Figure 2 &mdash; Wall body extrusion curved</p></td>
 
</tr>

</table>