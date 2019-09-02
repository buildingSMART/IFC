A duct fitting is a junction or transition in a ducted flow distribution system or used to connect duct segments, resulting in changes in flow characteristics to the fluid such as direction and flow rate.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcductfitting.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtype.htm">IfcDuctFittingType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDuctFitting Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_DuctFittingOccurrence.xml">Pset_DuctFittingOccurrence</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_DuctFittingPHistory.xml">Pset_DuctFittingPHistory</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifchvacdomain/Pset_DuctFittingTypeCommon.xml">Pset_DuctFittingTypeCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcDuctFitting Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifchvacdomain/Qto_DuctFittingBaseQuantities.xml">Qto_DuctFittingBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcDuctFitting Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Layer Set Usage

The [Material Layer Set Usage](../../templates/material-layer-set-usage.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the duct fitting is constructed.</td></tr>
<tr><td>Coating</td><td>The outer coating, if applicable.</td></tr>
<tr><td>Insulation</td><td>The insulating wrapping, if applicable.</td></tr>
<tr><td>Lining</td><td>The inner lining, if applicable.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcDuctFitting Material Layer Set Usage</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">BEND</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow inlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">BEND</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow outlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">CONNECTOR</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow inlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">CONNECTOR</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow outlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">ENTRY</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow outlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">EXIT</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow inlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">JUNCTION</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow inlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">JUNCTION</a></td><td>Outlet#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The left flow outlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">JUNCTION</a></td><td>Outlet#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The right flow outlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">OBSTRUCTION</a></td><td>Inlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow inlet.</td></tr>
<tr><td><a href="../../ifchvacdomain/lexical/ifcductfittingtypeenum.htm">OBSTRUCTION</a></td><td>Outlet</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The flow outlet.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcDuctFitting Port Nesting</p></td></tr></table>