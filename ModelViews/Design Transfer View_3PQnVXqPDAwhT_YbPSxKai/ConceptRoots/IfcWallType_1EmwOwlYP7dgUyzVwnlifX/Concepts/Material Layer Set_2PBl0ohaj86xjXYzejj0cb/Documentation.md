The material of the _IfcWallType_ is defined by the _IfcMaterialLayerSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcWallType_, if there is at least one occurrence of _IfcWallStandardCase_ for this type.

The shared material layer set definition is defined by assigning an _IfcMaterialLayerSet_ (see material use definition above). The _IfcMaterialLayer_ refers to one or several of _IfcMaterialLayer_ that is the common for all wall occurrence, if used. It is only applicable if the _IfcWallType_ has only occurrences of type _IfcWallStandardCase_ (see definition of _IfcWallStandardCase_ for further information).

> NOTE&nbsp; Since each individual instance of _IfcWallStandardCase_ defines its own _IfcMaterialLayerSetUsage_ including the offset from the wall axis, the same _IfcWallType_ can be used independently of the axis alignment of its occurrences.

If a wall type is decomposed into parts, then material layers of the _IfcWallType_ may be driven by corresponding material layers and profiles of components, where _IfcMaterialLayer_.Name refers to _IfcElement_.Name. The ordering of layers is preserved by the layer set, while the thicknesses of each layer are calculated according to the material layer/profile geometry of the parts.

The following is an example of a framed wall composition, where layers are ordered in the direction away from the viewer facing the right side of the wall:

<table class="gridtable">
<tr><th>#</th><th>Layer/Element Name</th><th>Element Type</th><th>Description</th></tr>
<tr><td>1</td><td>Forward Panels</td><td><i>IfcPlate</i></td><td>Panels on right side of wall (looking in direction of axis) such as gypsum board or cement board.</td></tr>
<tr><td>2</td><td>Frame</td><td><i>IfcElementAssembly</i></td><td>Framing, which is decomposed into tracks, studs, and insulation. The thickness of the layer is determined according to the greatest extent by superimposing the material layers and profiles of all aggregated objects (in the absense of this <i>IfcElementAssembly</i> having its own <i>IfcMaterialLayerSet</i> defining sequential positioning of elements).<br>
<table class="gridtable">
<tr><th>Element Name</th><th>Element Type</th><th>Material</th><th>Description</th></tr>
<tr><td>Track</td><td><i>IfcMemberStandardCase</i></td><td><i>IfcMaterialProfileSetUsage</i></td><td>Track at base and top of frame.</td></tr>
<tr><td>Stud</td><td><i>IfcMemberStandardCase</i></td><td><i>IfcMaterialProfileSetUsage</i></td><td>Studs, where <i>IfcMaterialProfileSetUsage</i>.ReferenceExtent defines the maximum height and <i>IfcMaterialProfileWithOffsets</i>.Offsets defines the stud spacing.</td></tr>
<tr><td>Insulation</td><td><i>IfcBuildingElementPart</i></td><td><i>IfcMaterialLayerSet</i></td><td>Insulation.</td></tr>
</table>

</td></tr>
<tr><td>3</td><td>Reverse Panels</td><td><i>IfcPlate</i></td><td>Panels on left side of wall (looking in direction of axis) such as gypsum board or cement board.</td></tr>
</table>