An _IfcPlate_ is a planar and often flat part with constant thickness. A plate may carry loads between or beyond points of support, or provide stiffening. The location of the plate (being horizontal, vertical or sloped) is not relevant to its definition (in contrary to _IfcWall_ and _IfcSlab_ (as floor slab)).

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1: thin, rigid, flat, metal product, of a thickness greater than that of a sheet.

Plates are normally made of steel, other metallic material, or by glass panels. However the definition of _IfcPlate_ is material independent and specific material information shall be handled by using _IfcAssociatesMaterial_ to assign a material specification to the _IfcPlate_.

> NOTE&nbsp; Although not necessarily, plates are often add-on parts. This is represented by the _IfcRelAggregates_ decomposition mechanism used to aggregate parts, such as _IfcPlate_, into a container element such as _IfcElementAssembly_ or _IfcCurtainWall_.

> NOTE&nbsp; The representation of a plate in a structural analysis model is provided by _IfcStructuralSurfaceMember_ being part of an _IfcStructuralAnalysisModel_.

An instance _IfcPlate_ should preferably get its geometric representation and material assignment through the type definition by _IfcPlateType_ assigned using the _IfcRelDefinesByType_ relationship. This allows identical plates in a construction to be represented by the same instance of _IfcPlateType_.

A plate may have openings, such as voids or recesses. They are defined by an _IfcOpeningElement_ attached to the plate using the inverse relationship _HasOpenings_ pointing to _IfcRelVoidsElement_. The position number of a plate as often used in steel construction is assigned through the attribute _IfcElement.Tag_

The IFC specification provides two entities for plate occurrences:

* _IfcPlateStandardCase_ used for all occurrences of plates, that are prismatic and where the thickness parameter can be fully described by the _IfcMaterialLayerSetUsage_. These plates are always represented geometrically by a 'SweptSolid' geometry (or by a 'Clipping' geometry based on 'SweptSolid'), if a 3D geometric representation is assigned. In addition they have to have a corresponding _IfcMaterialLayerSetUsage_ assigned.
* _IfcPlate_ used for all other occurrences of plates, particularly for plates with changing thickness, or plates with non planar surfaces, and plates having only 'SurfaceModel' or 'Brep' geometry.

> HISTORY&nbsp; New entity in IFC2x2

**_Geometric Representation_**

Currently, the <font color="#0000FF">'Surface'</font>, <font color="#0000FF">'FootPrint'</font>, 'Body', and 'Box' representations are supported. The 'Box' representation includes the representation type 'BoundingBox' and is explained at _IfcBuildingElement_.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcplate.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedbldgelements/lexical/ifcplatetype.htm">IfcPlateType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcPlate Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgelements/Pset_PlateCommon.xml">Pset_PlateCommon</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_ConcreteElementGeneral.xml">Pset_ConcreteElementGeneral</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementFabrication.xml">Pset_PrecastConcreteElementFabrication</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementGeneral.xml">Pset_PrecastConcreteElementGeneral</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcPlate Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcsharedbldgelements/Qto_PlateBaseQuantities.xml">Qto_PlateBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcPlate Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Layer Set

The [Material Layer Set](../../templates/material-layer-set.htm) concept applies to this entity.

The material of the _IfcPlate_ is defined by _IfcMaterialLayerSet_, or _IfcMaterial_, and it is attached either directly or at the _IfcPlateType_.

> NOTE&nbsp; It is illegal to assign an _IfcMaterialLayerSetUsage_ to an _IfcPlate_. Only the subtype _IfcPlateStandardCase_ supports this concept.

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Default spatial container </td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td><td>Spatial container for the element if it cannot be assigned to a building storey</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcsite.htm">IfcSite</a></td><td>Spatial container for the element in case that it is placed on site (outside of building)</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcPlate Spatial Containment</p></td></tr></table>

The _IfcPlate_, as any subtype of _IfcBuildingElement_, may participate alternatively in one of the two different containment relationships:

* the _Spatial Containment_ (defined here), or
* the _Element Composition_.

  
  
{ .use-head}
Surface 3D Geometry

The [Surface 3D Geometry](../../templates/surface-3d-geometry.htm) concept applies to this entity.

> NOTE&nbsp; The 'Surface' can be used to define a surfacic model of the building (e.g. for analytical purposes, or for reduced Level of Detail representation).

  
  
{ .use-head}
Body SweptSolid Geometry

The [Body SweptSolid Geometry](../../templates/body-sweptsolid-geometry.htm) concept applies to this entity.

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcArbitraryProfileDefWithVoids, IfcRectangleProfileDef, IfcCircleProfileDef, IfcEllipseProfileDef_ shall be supported.
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile.

{ .use-head}
Body Clipping Geometry

The [Body Clipping Geometry](../../templates/body-clipping-geometry.htm) concept applies to this entity.

  
  
{ .use-head}
Product Assignment

The [Product Assignment](../../templates/product-assignment.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcstructuralanalysisdomain/lexical/ifcstructuralsurfacemember.htm">IfcStructuralSurfaceMember</a></td><td>An idealized structural member corresponding to the plate.</td></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifctask.htm">IfcTask</a></td><td>A task for operating on the plate.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcPlate Product Assignment</p></td></tr></table>
