A waste terminal has the purpose of collecting or intercepting waste from one or more sanitary terminals or other fluid waste generating equipment and discharging it into a single waste/drainage system.

A waste terminal provides for all forms of trap and waste point that collects discharge from a sanitary terminal and discharges it into a waste/drainage subsystem or that collects waste from several terminals and passes it into a single waste/drainage subsystem. This includes the P and S traps from soil sanitary terminals, sinks, and basins as well as floor wastes and gully traps that provide collection points.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcwasteterminal.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltype.htm">IfcWasteTerminalType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcWasteTerminal Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeCommon.xml">Pset_WasteTerminalTypeCommon</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORTRAP</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeFloorTrap.xml">Pset_WasteTerminalTypeFloorTrap</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORWASTE</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeFloorWaste.xml">Pset_WasteTerminalTypeFloorWaste</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYSUMP</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeGullySump.xml">Pset_WasteTerminalTypeGullySump</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYTRAP</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeGullyTrap.xml">Pset_WasteTerminalTypeGullyTrap</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">ROOFDRAIN</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeRoofDrain.xml">Pset_WasteTerminalTypeRoofDrain</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTEDISPOSALUNIT</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeWasteDisposalUnit.xml">Pset_WasteTerminalTypeWasteDisposalUnit</a></td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTETRAP</a></td><td><a href="../../psd/ifcplumbingfireprotectiondomain/Pset_WasteTerminalTypeWasteTrap.xml">Pset_WasteTerminalTypeWasteTrap</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcWasteTerminal Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcplumbingfireprotectiondomain/Qto_WasteTerminalBaseQuantities.xml">Qto_WasteTerminalBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcWasteTerminal Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
<tr><td>Cover</td><td>Material from which the cover or grating is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcWasteTerminal Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORTRAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DRAINAGE</a></td><td>Drainage inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORTRAP</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DRAINAGE</a></td><td>Drainage outlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORWASTE</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Waste inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">FLOORWASTE</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Waste outlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYSUMP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYSUMP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Outlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYTRAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">GULLYTRAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Outlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">ROOFDRAIN</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">RAINWATER</a></td><td>Rainwater.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTEDISPOSALUNIT</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTEDISPOSALUNIT</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Outlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTETRAP</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Inlet.</td></tr>
<tr><td><a href="../../ifcplumbingfireprotectiondomain/lexical/ifcwasteterminaltypeenum.htm">WASTETRAP</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">WASTE</a></td><td>Outlet.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcWasteTerminal Port Nesting</p></td></tr></table>