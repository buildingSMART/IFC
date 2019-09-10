A filter is an apparatus used to remove particulate or gaseous matter from fluids and gases.

> HISTORY&nbsp; New entity in IFC4

{ .note}
> 

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionFlowElement_: [Axis Geometry](../../templates/axis-geometry.htm), [Clearance Geometry](../../templates/clearance-geometry.htm), [Lighting Geometry](../../templates/lighting-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcfilter.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertype.htm">IfcFilterType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcFilter Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_FilterPHistory.xml">Pset_FilterPHistory</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">AIRPARTICLEFILTER</a></td><td><a href="../../psd/ifchvacdomain/Pset_FilterTypeAirParticleFilter.xml">Pset_FilterTypeAirParticleFilter</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_FilterTypeCommon.xml">Pset_FilterTypeCommon</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">COMPRESSEDAIRFILTER</a></td><td><a href="../../psd/ifchvacdomain/Pset_FilterTypeCompressedAirFilter.xml">Pset_FilterTypeCompressedAirFilter</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">WATERFILTER</a></td><td><a href="../../psd/ifchvacdomain/Pset_FilterTypeWaterFilter.xml">Pset_FilterTypeWaterFilter</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcFilter Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifchvacdomain/Qto_FilterBaseQuantities.xml">Qto_FilterBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcFilter Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
<tr><td>Media</td><td>Material used for filtering particulates.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcFilter Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">AIRPARTICLEFILTER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">AIRCONDITIONING</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">AIRPARTICLEFILTER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">AIRCONDITIONING</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">COMPRESSEDAIRFILTER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">COMPRESSEDAIR</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">COMPRESSEDAIRFILTER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">COMPRESSEDAIR</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">ODORFILTER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">EXHAUST</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">ODORFILTER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">EXHAUST</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">OILFILTER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">OIL</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">OILFILTER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">OIL</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">STRAINER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DRAINAGE</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">STRAINER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DRAINAGE</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">WATERFILTER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DOMESTICCOLDWATER</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcfiltertypeenum.htm">WATERFILTER</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DOMESTICCOLDWATER</a></td><td>Outgoing fluid.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcFilter Port Nesting</p></td></tr></table>
