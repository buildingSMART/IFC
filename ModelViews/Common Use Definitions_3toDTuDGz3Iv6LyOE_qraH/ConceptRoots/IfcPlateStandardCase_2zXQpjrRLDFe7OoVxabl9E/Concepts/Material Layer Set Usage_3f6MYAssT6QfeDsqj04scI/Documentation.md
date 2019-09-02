The material of the _IfcPlateStandardCase_ is defined by _IfcMaterialLayerSetUsage_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Multi-layer plates can be represented by refering to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_ that is referenced from the _IfcMaterialLayerSetUsage_.&nbsp;

Material information can also be given at the _IfcPlateType_, defining the common attribute data for all occurrences of the same type.&nbsp;It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _IfcPlateType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_.

The _IfcPlateStandardCase_ defines in addition that the _IfcPlateType_ should have a unique _IfcMaterialLayerSet_, that is referenced by the&nbsp;_IfcMaterialLayerSetUsage_ assigned to all occurrences of this _IfcPlateType_.

Figure 1 illustrates assignment of _IfcMaterialLayerSetUsage_ and _IfcMaterialLayerSet_ to the _IfcPlateStandardCase_ as the plate occurrence and to the _IfcPlateType_. The same _IfcMaterialLayerSet_ shall be shared by many occurrences of _IfcMaterialLayerSetUsage_. This relationship shall be consistent to the relationship between the _IfcPlateType_ and the _IfcPlateStandardCase_.

<table border="0" cellpadding="2" cellspacing="2">

<tr><td width="610" align="left" valign="top">
<p><img src="../../../figures/IfcSlab_MaterialUsage-01.png" alt="Material layer set and usage" height="220" width="501">&nbsp;</p></td></tr>

<tr><td><p class="figure">Figure 1 &mdash; Plate type definition</p></td></tr>

</table>

As shown in Figure 106, the following conventions shall be met:

* The reference coordinate system is the coordinate system established by the _IfcExtrudedAreaSolid.Position_.
* The reference plane is the plane defined by the extruded profile of _IfcExtrudedAreaSolid.SweptSolid_. The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is given as a distance from this plane.
* The _IfcMaterialLayerSetUsage.DirectionSense_ defines how the _IfcMaterialLayer_'s are assigned to the reference plane. POSITIVE means in direction to the positive z-axis of the reference coordinate system.
* The _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ is the distance parallel to the reference plane and always perpendicular to the base (XY) plane of the reference coordinate system. This is independent of a potential non-perpendicular extrusion given by _IfcExtrudedAreaSolid.ExtrudedDirection_ &lt;&gt; 0.,0.,1. A positive value of _IfcMaterialLayerSetUsage.OffsetFromReferenceLine_ would then point into the positive z-axis of the reference coordinate system.
* The _Thickness_ of each _IfcMaterialLayer_ shall be the parallel distance (measured perpendicular to the base plane). The _TotalThickness_ of the _IfcMaterialLayerSet_ is the sum of all layer thicknesses and in case of a perpendicular extrusion identical with _IfcExtrudedAreaSolid.Depth_
* The _IfcMaterialLayerSetUsage.LayerSetDirection_ i always AXIS3.

!["plate material layer set"](../../../figures/IfcMaterialLayerSetUsage_Slab-01.png "Figure 2 &mdash; Plate material layers")