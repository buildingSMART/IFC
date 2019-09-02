The material of _IfcWall_ can be defined by _IfcMaterialLayerSetUsage_ and attached by _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Multi-layer walls can be represented by refering to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_ that is referenced from the _IfcMaterialLayerSetUsage_.

When assigning an _IfcMaterialLayerSetUsage_ to _IfcWall_ it shall imply that the _IfcWallType_ should have a unique _IfcMaterialLayerSet_, that is referenced by _IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcWallType_.

<table>
 
<tr>
  <td><img src="../../../figures/ifcwall_materialusage-01.png" alt="Material layer set and usage" height="220" width="501"></td>
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
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is the distance parallel to the reference axis and always within the base (XY) plane of the reference coordinate system. A positve value of _IfcMaterialLayerSetUsage_.OffsetFromReferenceLine would then point into the positive y-axis of the reference coordinate system.
* The _IfcMaterialLayerSetUsage_.DirectionSense defines how the _IfcMaterialLayer_'s are assigned to the reference axis. POSITIVE means in direction to the positive y-axis of the reference coordinate system.
* The _Thickness_ of each _IfcMaterialLayer_ is provided starting from the _OffsetFromReferenceLine_ and in the direction given by _DirectionSense_. It is applied without any gap or overlap between two consecutive layers. The _TotalThickness_ of the _IfcMaterialLayerSet_ is the sum of all layer thicknesses.
* The _IfcMaterialLayerSetUsage.LayerSetDirection_ is always AXIS2.

!["wall material layer set"](../../../figures/ifcmateriallayersetusage_wall-01.png "Figure 2 &mdash; Wall material layers")