A stair flight is an assembly of building components in a single "run" of stair steps (not interrupted by a landing). The stair steps and any stringers are included in the stair flight. A winder is also regarded a part of a stair flight.

An _IfcStairFlight_ is normally aggregated by an _IfcStair_ through the _IfcRelAggregates_ relationship, the stair flight is then included in the set of _IfcRelAggregates.RelatedObjects_. An _IfcStairFlight_ normally connects the floor slab of zero to two different storeys (or partial storeys, or landings) within a building. The connection relationship between the _IfcStairFlight_ and the _IfcSlab_ is expressed using the _IfcRelConnectsElements_ relationship.

> HISTORY&nbsp; New entity in IFC2.0.

Currently, the 'Axis', 'FootPrint', 'Body', and 'Box' representations are supported. The 'Box' representation includes the representation type 'BoundingBox' and is explained at _IfcBuildingElement_.

* **Axis**: A two-dimensional open curve _IfcBoundedCurve_ defining the walking line for the stair flight.
* **FootPrint**: A geometric curve set defining the footing print, including the boundary of the stair flight.
* **Body**: A solid representation defining the 3D shape of the stair flight

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcBuildingElement_: [Product Assignment](../../templates/product-assignment.htm), [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcstairflight.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedbldgelements/lexical/ifcstairflighttype.htm">IfcStairFlightType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcStairFlight Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgelements/Pset_StairFlightCommon.xml">Pset_StairFlightCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcStairFlight Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcsharedbldgelements/Qto_StairFlightBaseQuantities.xml">Qto_StairFlightBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcStairFlight Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Single

The [Material Single](../../templates/material-single.htm) concept applies to this entity.

The material of the _IfcStairFlight_ is defined by the _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Default spatial container, if the stair  flight is not used (by default) as a part within a stair container.</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td><td>Spatial container for the element if it cannot be assigned to a building storey.</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcsite.htm">IfcSite</a></td><td>Spatial container for the element in case that it is placed on site (outside of building)</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcStairFlight Spatial Containment</p></td></tr></table>

The _IfcStairFlight_, as any subtype of _IfcBuildingElement_, may participate alternatively in one of the two different containment relationships:

* the _Spatial Containment_ (defined here), or
* the _Element Composition_.

> NOTE&nbsp; Model view definitions or implementer agreements may force an _IfcStairFlight_ to be solely used as a part within an _IfcStair_ container. In this case, no _Spatial containment_ shall be used.

  
  
{ .use-head}
Axis 2D Geometry

The [Axis 2D Geometry](../../templates/axis-2d-geometry.htm) concept applies to this entity.

The walking line is represented by a two-dimensional open curve as the axis. The curve is directed into the upward direction (direction has to be interpreted as specified at the subtypes of _IfcCurve_).

Figure 1 illustrates the axis representation which has the following constraints:

* In case of straight flights the curve shall be a single item of type _IfcPolyline_.
* In case of winding flights the curve shall be a single item of type _IfcCompositeCurve_.
* In case of a curved flight or a spiral flight the curve shall be a single item of type _IfcTrimmedCurve_.

!["walking line"](../../../figures/IfcStairFlight_01-Layout1.gif "Figure 1 &mdash; Stair flight axis")

  
  
{ .use-head}
FootPrint Geometry

The [FootPrint Geometry](../../templates/footprint-geometry.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>FootPrint</td><td>GeometricCurveSet</td><td>&nbsp;</td><td>Any collection of points and curves representing the floor plan projection.</td></tr>
<tr><td>FootPrint</td><td>Annotation2D</td><td>&nbsp;</td><td>Any collection of points and curves, and additional hatching and text representing the floor plan projection.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcStairFlight FootPrint Geometry</p></td></tr></table>

The flight foot print, including the flight boundary is represented by a two-dimensional geometric curve set.

Figure 2 illustrates the footprint representation which has the following constraints:

* In case of straight flights the curve set shall consists of a single item of type _IfcPolyline_.
* In case of winding flights or curved flights the curve set shall consists of a single item of type _IfcCompositeCurve_.
* In case of a spiral flight the curve set shall consists of a single item of type _IfcConic_ or _IfcPolyline_.

!["boundary"](../../../figures/IfcStairFlight_02-Layout1.gif "Figure 2 &mdash; Stair flight footprint")

  
  
{ .use-head}
Body SweptSolid Geometry

The [Body SweptSolid Geometry](../../templates/body-sweptsolid-geometry.htm) concept applies to this entity.

Figure 3 illustrates the 'Body' geometric representation using a 'SweptSolid' representation type.

!["3D"](../../../figures/IfcStairFlight_03-Layout1.gif "Figure 3 &mdash; Stair flight body")