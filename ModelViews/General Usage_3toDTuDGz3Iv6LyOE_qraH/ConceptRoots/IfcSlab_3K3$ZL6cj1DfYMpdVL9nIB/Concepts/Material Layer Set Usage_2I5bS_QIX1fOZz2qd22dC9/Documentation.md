The material of _IfcSlab_ can be defined by _IfcMaterialLayerSetUsage_ and attached by _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Multi-layer slabs can be represented by refering to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_ that is referenced from th e _IfcMaterialLayerSetUsage_.

When assigning an _IfcMaterialLayerSetUsage_ to _IfcSlab_ it shall imply that the _IfcSlabType_ should have a unique _IfcMaterialLayerSet_, that is referenced by _IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcSlabType_.

<table>

 <tr>
  <td><img src="../../../figures/ifcslab_materialusage-01.png" alt="Material layer set and usage" height="220" width="501"></td>
  
<td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialLayerSetUsage</em> and <em>IfcMaterialLayerSet</em> to the <em>IfcSlab</em> as the slab occurrence and to the <em>IfcSlabType</em>. The same <em>IfcMaterialLayerSet</em> shall be shared by many occurrences of <em>IfcMaterialLayerSetUsage</em>. This relationship shall be consistent to the relationship between the <em>IfcSlabType</em> and the <em>IfcSlabStandardCase</em>.</blockquote></td>
 </tr>
 
<tr><td><p class="figure">Figure 1 &mdash; Slab type definition</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

Figure 2 illustrates slab material usage, where the following conventions shall be met:

* The reference coordinate system is the coordinate system established by the _IfcExtrudedAreaSolid.Position_.
* The reference plane is the plane defined by the extruded profile of _IfcExtrudedAreaSolid.SweptSolid_. The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is given as a distance from this plane.
* The _IfcMaterialLayerSetUsage.DirectionSense_ defines how the _IfcMaterialLayer_'s are assigned to the reference plane. POSITIVE means in direction to the positive z-axis of the reference coordinate system.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is the distance parallel to the reference plane and always perpendicular to the base (XY) plane of the reference coordinate system. This is independent of a potential non-perpendicular extrusion given by _IfcExtrudedAreaSolid.ExtrudedDirection_ &lt;&gt; 0.,0.,1. A positive value of _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ would then point into the positive z-axis of the reference coordinate system.
* The _Thickness_ of each _IfcMaterialLayer_ shall be the parallel distance (measured perpendicular to the base plane). The _TotalThickness_ of the _IfcMaterialLayerSet_ is the sum of all layer thicknesses and in case of a perpendicular extrusion identical with _IfcExtrudedAreaSolid.Depth_
* The _IfcMaterialLayerSetUsage.LayerSetDirection_ is always AXIS3.

<table summary="material use definition for standard slabs">

 <tr>
  <td align="left" valign="top" width="610">
<img src="../../../figures/ifcmateriallayersetusage_slab-01.png" alt="slab material layer set" width="601" height="321" border="0">
</td></tr>
<tr><td align="left" valign="top" width="610">
<img src="../../../figures/ifcmateriallayersetusage_roofslab-01.png" alt="roof slab material layer set" width="600" height="400" border="0"></td></tr>
<tr><td><p class="figure">Figure 2 &mdash; Slab material layers</p></td></tr>
</table>