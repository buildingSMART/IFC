The building storey has an elevation and typically represents a (nearly) horizontal aggregation of spaces that are vertically bound.

A storey is (if specified) associated to a building. A storey may span over several connected storeys. Therefore storey complex provides for a collection of storeys included in a building. A storey can also be decomposed in (horizontical) parts, where each part defines a partial storey. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElements_ which is interpreted as follow:

* **COMPLEX**: building storey complex
* **ELEMENT**: building storey
* **PARTIAL**: partial building storey

> EXAMPLE&nbsp; In split level houses, a storey is split into two or more partial storeys, each with a different elevation. It can be handled by defining a storey, which includes two or more partial storeys with the individual elevations.

The _IfcBuildingStorey_ is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship _IfcRelAggregates_.

Figure 1 shows the _IfcBuildingStorey_ as part of the s patial structure. It also serves as the spatial container for building and other elements.

> NOTE&nbsp; Detailed requirements on mandatory element containment and placement structure relationships are given in view definitions and implementer agreements.

!["IfcBuildingStorey as part of a spatial structure"](../../../figures/IfcBuildingStorey-SpatialStructure.png "Figure 1 &mdash; Building storey composition")

> HISTORY&nbsp; New entity in IFC1.0

{ .use-head}
Attribute Use Definition

Figure 2 describes the heights and elevations of the _IfcBuildingStorey_.

* elevation of storey provided by: _IfcBuildingStorey.Elevation_ as a local height value relative to _IfcBuilding.ElevationOfRefHeight_, it is usually the top of construction slab
* net height of storey, also referred to as total height or system height (top of construction slab to top of construction slab above): provided by BaseQuantity with Name="GrossHeight"
* net height of storey (top of construction slab to bottom of construction slab above): provided by BaseQuantity with Name="NetHeight"

<table summary="attributes" cellpadding="2" cellspacing="2">
<tbody>
<tr>
<td align="left" valign="top"><img src="../../../figures/IfcBuildingStorey_Heights.png" alt="space heights" border="0" height="400" width="450"></td>
<td align="left" valign="top"></td></tr>
<tr><td><p class="figure">Figure 2 &mdash; Building storey elevations</p></td></tr>
</tbody>
</table>

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcbuildingstorey.htm)

{ .use-head}
Spatial Composition

The [Spatial Composition](../../templates/spatial-composition.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Spatial Composite</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td><td>Assignment to the building, where the building storey is a part of.</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Assignment to another building storey, e.g. if this building storey is a partial storey that refer to another storey.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcBuildingStorey Spatial Composition</p></td></tr></table>

> NOTE&nbsp; By using the inverse relationship _IfcBuildingStorey.Decomposes_ it references (_IfcBuilding_ || _IfcBuildingStorey_) through _IfcRelAggregates.RelatingObject_IfcBuildingStorey_, the referenced 
_IfcBuildingStorey_ needs to have a different and higher
 _CompositionType_, i.e. COMPLEX (if the other _IfcBuildingStorey_ has ELEMENT), or ELEMENT (if the other
 _IfcBuildingStorey_ has PARTIAL)._

  
  
{ .use-head}
Spatial Decomposition

The [Spatial Decomposition](../../templates/spatial-decomposition.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Spatial Parts</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcspace.htm">IfcSpace</a></td><td>Reference to the spaces that are assigned to this storey. </td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Spatial decomposition into partial stories, if this storey is a main storey having subdivisions.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcBuildingStorey Spatial Decomposition</p></td></tr></table>

> NOTE&nbsp; By using the inverse relationship _IfcBuildingStorey.IsDecomposedBy_ it references _IfcBuildingStorey_ || _IfcSpace_ through _IfcRelAggregates.RelatedObjects_. If it refers to another instance of _IfcBuildingStorey_, the referenced _IfcBuildingStorey_ needs to have a different and lower _CompositionType_, i.e. ELEMENT (if the other _IfcBuildingStorey_ has COMPLEX), or PARTIAL (if the other _IfcBuildingStorey_ has ELEMENT).

> NOTE&nbsp; Multi storey spaces shall be spatially contained by only a single building storey, usually it is the building storey where the base of the space lies.

  
  
{ .use-head}
Spatial Container

The [Spatial Container](../../templates/spatial-container.htm) concept applies to this entity.

If there are building elements and/or other elements directly related to the _IfcBuildingStorey_ (like most building elements, such as walls, columns, etc.), they are associated with the _IfcBuildingStorey_ by using the objectified relationship _IfcRelContainedInSpatialStructure_. The _IfcBuildingStorey_ references them by its inverse relationship:

* _IfcBuildingStorey.ContainsElements_ -- referencing any subtype of _IfcProduct_ (with the exception of other spatial structure element) by _IfcRelContainedInSpatialStructure.RelatedElements_.

Elements can also be referenced in an _IfcBuildingStorey_, for example, if they span through several storeys. This is expressed by using the objectified relationship _IfcRelReferencedInSpatialStructure_. Systems, such as building service or electrical distribution systems, zonal systems, or structural analysis systems, relate to _IfcBuildingStorey_ by using the objectified relationship _IfcRelServicesBuildings_.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_BuildingStoreyCommon.xml">Pset_BuildingStoreyCommon</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_PropertyAgreement.xml">Pset_PropertyAgreement</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_AirSideSystemInformation.xml">Pset_AirSideSystemInformation</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_SpaceFireSafetyRequirements.xml">Pset_SpaceFireSafetyRequirements</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_SpaceLightingRequirements.xml">Pset_SpaceLightingRequirements</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_SpaceOccupancyRequirements.xml">Pset_SpaceOccupancyRequirements</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_SpaceThermalRequirements.xml">Pset_SpaceThermalRequirements</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_ThermalLoadAggregate.xml">Pset_ThermalLoadAggregate</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_ThermalLoadDesignCriteria.xml">Pset_ThermalLoadDesignCriteria</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcBuildingStorey Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcproductextension/Qto_BuildingStoreyBaseQuantities.xml">Qto_BuildingStoreyBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcBuildingStorey Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity.

The local placement for _IfcBuildingStorey_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if relative placement is used) to the _IfcSpatialStructureElement_ of type _IfcBuilding_, or of type _IfcBuildingStorey_ (e.g. to position a building storey relative to a building storey complex, or a partial building storey to a building storey).
* If the relative placement is not used, the absolute placement is defined within the world coordinate system.

  
  
{ .use-head}
FootPrint GeomSet Geometry

The [FootPrint GeomSet Geometry](../../templates/footprint-geomset-geometry.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>FootPrint</td><td>GeometricCurveSet</td><td><a href="../../ifcgeometricmodelresource/lexical/ifcgeometriccurveset.htm">IfcGeometricCurveSet</a></td><td>Set of curves (outer and inner) representing the floor projection,</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcBuildingStorey FootPrint GeomSet Geometry</p></td></tr></table>

The foot print representation of _IfcBuildingStorey_ is given by either a single 2D curve (such as _IfcPolyline_ or _IfcCompositeCurve_), or by a list of 2D curves (in case of inner boundaries), if the building storey has an independent geometric representation.

> NOTE&nbsp; The independent geometric representation of _IfcBuildingStorey_ may not be allowed in certain model view definitions. In those cases only the contained elements and spaces have an independent geometric representation.

  
  
{ .use-head}
Body Geometry

The [Body Geometry](../../templates/body-geometry.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcBuildingStorey Body Geometry</p></td></tr></table>

The body (or solid model) geometric representation (if the building storey has an independent geometric representation) of _IfcBuildingStorey_ is defined using faceted B-Rep capabilities (with or without voids), based on the _IfcFacetedBrep_ or on the _IfcFacetedBrepWithVoids_.

> NOTE&nbsp; Since the building storey shape is usually described by the exterior building elements, an independent shape representation shall only be given, if the building storey is exposed independently from its constituting elements and such independent geometric representation may be prohibited in model view definitions.