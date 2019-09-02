The distribution element _IfcDistributionFlowElement_ defines occurrence elements of a distribution system that facilitate the distribution of energy or matter, such as air, water or power.

> EXAMPLE&nbsp; Examples of distribution flow elements are ducts, pipes, wires, fittings, and equipment.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Ports are now primarily defined using _IfcRelNests_ to enable definition of ports at type definitions (both forward and backward compatible), provide a logical order, and reduce the number of relationship objects needed. The relationship _IfcRelConnectsPortToElement_ is still supported, however is now specific to dynamically connected ports.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Quantity Sets](../../templates/quantity-sets.htm), [Spatial Containment](../../templates/spatial-containment.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcdistributionflowelement.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDistributionFlowElement Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_SoundGeneration.xml">Pset_SoundGeneration</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_ElectricalDeviceCommon.xml">Pset_ElectricalDeviceCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcDistributionFlowElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Axis Geometry

The [Axis Geometry](../../templates/axis-geometry.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcDistributionFlowElement Axis Geometry</p></td></tr></table>

This represents the 3D flow path of the item having _IfcShapeRepresentation.RepresentationType_ of 'Curve3D' and containing a single _IfcBoundedCurve_ subtype such as _IfcPolyline_, _IfcTrimmedCurve_, or _IfcCompositeCurve_. For elements containing directional ports (_IfcDistributionPort_ with _FlowDirection_ of _SOURCE_ or _SINK_), the direction of the curve indicates direction of flow where a _SINK_ port is positioned at the start of the curve and a _SOURCE_ port is positioned at the end of the curve. This representation is most applicable to flow segments (pipes, ducts, cables), however may be used at other elements to define a primary flow path if applicable.

  
  
{ .use-head}
Clearance Geometry

The [Clearance Geometry](../../templates/clearance-geometry.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcDistributionFlowElement Clearance Geometry</p></td></tr></table>

This represents the 3D clearance volume of the item having RepresentationType of 'Surface3D'. Such clearance region indicates space that should not intersect with the 'Body' representation of other elements, though may intersect with the 'Clearance' representation of other elements. The particular use of clearance space may be for safety, maintenance, or other purposes.

  
  
{ .use-head}
Lighting Geometry

The [Lighting Geometry](../../templates/lighting-geometry.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>LightSource</td><td>&nbsp;</td></tr>
<tr><td>&nbsp;</td><td>MappedRepresentation</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcDistributionFlowElement Lighting Geometry</p></td></tr></table>

This represents the light emission of the item having _IfcShapeRepresentation.RepresentationType_ of 'LightSource' and containing one or more _IfcLightSource_ subtypes. This representation is most applicable to lamps and light fixtures, however may be used at other elements that emit light.