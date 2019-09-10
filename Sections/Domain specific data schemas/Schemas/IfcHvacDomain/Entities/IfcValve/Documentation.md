A valve is used in a building services piping distribution system to control or modulate the flow of the fluid.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcvalve.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetype.htm">IfcValveType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcValve Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_ValvePHistory.xml">Pset_ValvePHistory</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">AIRRELEASE</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeAirRelease.xml">Pset_ValveTypeAirRelease</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeCommon.xml">Pset_ValveTypeCommon</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DRAWOFFCOCK</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeDrawOffCock.xml">Pset_ValveTypeDrawOffCock</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">FAUCET</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeFaucet.xml">Pset_ValveTypeFaucet</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">FLUSHING</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeFlushing.xml">Pset_ValveTypeFlushing</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">GASTAP</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeGasTap.xml">Pset_ValveTypeGasTap</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">ISOLATING</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeIsolating.xml">Pset_ValveTypeIsolating</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">MIXING</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypeMixing.xml">Pset_ValveTypeMixing</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">PRESSUREREDUCING</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypePressureReducing.xml">Pset_ValveTypePressureReducing</a></td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">PRESSURERELIEF</a></td><td><a href="../../psd/ifchvacdomain/Pset_ValveTypePressureRelief.xml">Pset_ValveTypePressureRelief</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcValve Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifchvacdomain/Qto_ValveBaseQuantities.xml">Qto_ValveBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcValve Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
<tr><td>Operation</td><td>Material from which the operating mechanism (such as gate, globe, plug, needle, or clack) of the valve is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcValve Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Connectivity

The [Connectivity](../../templates/connectivity.htm) concept applies to this entity as shown in Table 593.

{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">AIRHANDLER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">ANTIVACUUM</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">CHANGEOVER</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">CHANGEOVER</a></td><td>Outlet#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Switched outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">CHANGEOVER</a></td><td>Outlet#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Switched outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">CHECK</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">CHECK</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">COMMISSIONING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">COMMISSIONING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DIVERTING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DIVERTING</a></td><td>Outlet#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DIVERTING</a></td><td>Outlet#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DOUBLECHECK</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DOUBLECHECK</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DOUBLEREGULATING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DOUBLEREGULATING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">DRAWOFFCOCK</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">FAUCET</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">FLUSHING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">FLUSHING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">GASCOCK</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">GAS</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">GASTAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">GAS</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">ISOLATING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">GAS</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">ISOLATING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">GAS</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">MIXING</a></td><td>Inlet#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid to be mixed.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">MIXING</a></td><td>Inlet#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid to be mixed.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">MIXING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">PRESSUREREDUCING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">PRESSUREREDUCING</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">PRESSURERELIEF</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">REGULATING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">REGULATING</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">SAFETYCUTOFF</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">SAFETYCUTOFF</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">STEAMTRAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">STEAMTRAP</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Outgoing fluid.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcvalvetypeenum.htm">STOPCOCK</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>Incoming fluid.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcValve Port Nesting</p></td></tr></table>
