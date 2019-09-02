A surface feature is a modification at (onto, or into) of the surface of an element. Parts of the surface of the entire surface may be affected. The volume and mass of the element may be increased, remain unchanged, or be decreased by the surface feature, depending on manufacturing technology. However, any increase or decrease of volume is small compared to the total volume of the element.

The standard use of instances of _IfcSurfaceFeature_ is as a part of element type objects (instances of subtypes of _IfcElementType_). The part&ndash;whole relationship is established by an aggregation relationship object, expressing the decomposition of an element type into one or more additive elements (element parts) and zero or more feature elements.

> HISTORY&nbsp; New entity in IFC4.

****Containment Use Definition****:

Surface features shall have no spatial containment relationship to the spatial structure since they are dependent on element types without spatial containment relationships or on an element occurrence with own spatial containment relationship.

* The _SELF\IfcElement.ContainedInStructure_ relationship shall be NIL.

****Geometry use definition****:

The geometric representation of _IfcSurfaceFeatureElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcSurfaceFeatureElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* In case of features which are part of an element type, absolute placement into the type object's implied coordinate system shall be used.
* In case of features which are voiding an element occurrence, the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the respective element.

**Shape representation**

Different shape representations may be used, depending on the nature of the feature and information requirements:

* Symbolic representation, such as the two-dimensional bounding box of a tag. 
* A geometric set representing the geometric items of a mark.
* Surface representations of treated parts of the lement surface by means of _IfcShellBasedSurfaceModel_. The faces within the surface model may be included into a B-Rep model within a representation map of the parent element type.

Higher-level parameters (geometric and non-geometric) may be provided by property sets based on local agreements.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcFeatureElement_: [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcsurfacefeature.htm)

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
<tr><td><p class="table">Table 1 &mdash; IfcSurfaceFeature Property Sets for Objects</p></td></tr></table>

  
  
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
<tr><td><p class="table">Table 2 &mdash; IfcSurfaceFeature Product Placement</p></td></tr></table>

The local placement for _IfcSurfaceFeatureElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* In case of features which are part of an element type, absolute placement into the type object's implied coordinate system shall be used.
* In case of features which are voiding an element occurrence, the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the respective element.

  
  
{ .use-head}
Body Geometry

The [Body Geometry](../../templates/body-geometry.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>Surface representations of treated parts of the lement surface by means of <em>IfcShellBasedSurfaceModel</em>.  The faces within the surface model may be included into a B-Rep model within a representation map of the parent element type.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcSurfaceFeature Body Geometry</p></td></tr></table>