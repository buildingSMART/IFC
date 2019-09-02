A voiding feature is a modification of an element which reduces its volume. Such a feature may be manufactured in different ways, for example by cutting, drilling, or milling of members made of various materials, or by inlays into the formwork of cast members made of materials such as concrete.

The standard use of instances of _IfcVoidingFeature_ is as a part of element type objects (instances of subtypes of _IfcElementType_). The part&ndash;whole relationship is established by an aggregation relationship object, expressing the decomposition of an element type into one or more additive elements (element parts) and zero or more feature elements.

> HISTORY&nbsp; New entity in IFC4.

{ .use-head}
Containment Use Definition

Voiding features shall have no spatial containment relationship to the spatial structure since they are dependent on element types without spatial containment relationships or on an element occurrence with own spatial containment relationship.

* The _SELF\IfcElement.ContainedInStructure_ relationship shall be NIL.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcFeatureElement_: [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcvoidingfeature.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Condition.xml">Pset_Condition</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactIndicators.xml">Pset_EnvironmentalImpactIndicators</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactValues.xml">Pset_EnvironmentalImpactValues</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerOccurrence.xml">Pset_ManufacturerOccurrence</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerTypeInformation.xml">Pset_ManufacturerTypeInformation</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedmgmtelements/Pset_PackingInstructions.xml">Pset_PackingInstructions</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLife.xml">Pset_ServiceLife</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Warranty.xml">Pset_Warranty</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcVoidingFeature Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Relative</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>Relative placement according to position and rotation relative to container.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifclocalplacement.htm">IfcLocalPlacement</a></td><td>&nbsp;</td><td>Absolute placement according to position and rotation of world coordinate system.</td></tr>
<tr><td><a href="../../ifcgeometricconstraintresource/lexical/ifcgridplacement.htm">IfcGridPlacement</a></td><td>&nbsp;</td><td>Placement according to grid intersection.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcVoidingFeature Product Placement</p></td></tr></table>

The local placement for _IfcVoidingFeatureElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* In case of features which are part of an element type, absolute placement into the type object's implied coordinate system shall be used.
* In case of features which are voiding an element occurrence, the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the respective element.

  
  
{ .use-head}
Profile Geometry

The [Profile Geometry](../../templates/profile-geometry.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>Symbolic representations may be used for simple shapes such as holes or edge features.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcVoidingFeature Profile Geometry</p></td></tr></table>

  
  
{ .use-head}
Surface Geometry

The [Surface Geometry](../../templates/surface-geometry.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcVoidingFeature Surface Geometry</p></td></tr></table>

  
  
{ .use-head}
Body Geometry

The [Body Geometry](../../templates/body-geometry.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>Volumetric representations may be used to semi-parametrically model the actual volume of the void created by the feature.  Attributes in the shape model directly correspond with feature parameters, for example diameter of circular holes or length and width of cutouts.  The objects within the shape model of the feature's shape representation can be included into a CSG model within a representation map of the parent element type.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcVoidingFeature Body Geometry</p></td></tr></table>