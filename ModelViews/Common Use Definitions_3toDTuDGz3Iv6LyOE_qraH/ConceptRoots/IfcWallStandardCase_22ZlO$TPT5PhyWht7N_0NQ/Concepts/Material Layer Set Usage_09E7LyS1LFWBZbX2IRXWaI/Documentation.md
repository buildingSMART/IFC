Multi-layer walls can be represented by refering to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_ that is referenced from the _IfcMaterialLayerSetUsage_.&nbsp;

Material information can also be given at the _IfcWallType_, defining the common attribute data for all occurrences of the same type. It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _IfcSlabType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_.

The _IfcWallType_ should then have a unique _IfcMaterialLayerSet_, that is referenced by the _IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcWallType_.

&nbsp;

<table>
 
<tr>
  <td><img src="../../../figures/IfcWallStandardCase_MaterialUsage-01.png" alt="Material layer set and usage" height="220" width="501"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates assignment of <em>IfcMaterialLayerSetUsage</em> and <em>IfcMaterialLayerSet</em> to the wall type and the wall occurrence.</blockquote></td>
 </tr>

 <tr>
  <td><p class="figure">Figure 1 &mdash; Wall Standard Object Typing</p></td>
  <td>&nbsp;</td>
 </tr>

</table>

Figure 2 illustrates material layer usage, where the following conventions shall be met:

* The reference coordinate system is the local coordinate system established by the _ObjectPlacement_ of the _IfcWallStandardCase_.
* The reference axis is the axis defined by the _IfcShapeRepresentation_ with _RepresentationType_='Axis' as one of the _Representation.Representations_ of the _IfcWallStandardCase_.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is given as a distance from this axis.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is the distance parallel to the reference axis and always within the base (XY) plane of the reference coordinate system. A positve value of _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ would then point into the positive y-axis of the reference coordinate system.
* The _IfcMaterialLayerSetUsage.DirectionSense_ defines how the _IfcMaterialLayer_'s are assigned to the reference axis. POSITIVE means in direction to the positive y-axis of the reference coordinate system.
* The _Thickness_ of each _IfcMaterialLayer_ is provided starting from the _OffsetFromReferenceLine_ and in the direction given by _DirectionSense_. It is applied without any gap or overlap between two consecutive layers. The _TotalThickness_ of the _IfcMaterialLayerSet_ is the sum of all layer thicknesses.
* The _IfcMaterialLayerSetUsage.LayerSetDirection_ is always AXIS2.

!["roof slab material layer set"](../../../figures/IfcMaterialLayerSetUsage_Wall-01.png "Figure 2 &mdash; Wall material layers")