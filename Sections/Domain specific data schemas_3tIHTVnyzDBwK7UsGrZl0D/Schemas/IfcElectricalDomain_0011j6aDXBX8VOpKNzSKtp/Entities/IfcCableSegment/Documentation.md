A cable segment is a flow segment used to carry electrical power, data, or telecommunications signals.

A cable segment is used to typically join two sections of an electrical network or a network of components carrying the electrical service.

> HISTORY&nbsp; New entity in IFC4

{ .note}
> 

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionFlowElement_: [Clearance Geometry](../../templates/clearance-geometry.htm), [Lighting Geometry](../../templates/lighting-geometry.htm)
* _IfcFlowSegment_: [Axis Geometry](../../templates/axis-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifccablesegment.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttype.htm">IfcCableSegmentType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcCableSegment Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">BUSBARSEGMENT</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentTypeBusBarSegment.xml">Pset_CableSegmentTypeBusBarSegment</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">CABLESEGMENT</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentTypeCableSegment.xml">Pset_CableSegmentTypeCableSegment</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentTypeCommon.xml">Pset_CableSegmentTypeCommon</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">CONDUCTORSEGMENT</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentTypeConductorSegment.xml">Pset_CableSegmentTypeConductorSegment</a></td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">CORESEGMENT</a></td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentTypeCoreSegment.xml">Pset_CableSegmentTypeCoreSegment</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_CableSegmentOccurrence.xml">Pset_CableSegmentOccurrence</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcCableSegment Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcelectricaldomain/Qto_CableSegmentBaseQuantities.xml">Qto_CableSegmentBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcCableSegment Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Profile Set Usage

The [Material Profile Set Usage](../../templates/material-profile-set-usage.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Conductor</td><td>Material from which the conductors are constructed, such as Aluminium or Copper.</td></tr>
<tr><td>Insulation</td><td>The material from which the insulation is constructed such as PVC, PEX, or EPR.</td></tr>
<tr><td>Screen</td><td>The material from which the screen that covers the sheath is constructed (mantel) such as Aluminium, Copper, Steel, or Lead.</td></tr>
<tr><td>Sheath</td><td>The outer sheathing of the cable which may be color-coded.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcCableSegment Material Profile Set Usage</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">CABLESEGMENT</a></td><td><a href="../../ifcelectricaldomain/lexical/ifccablesegment.htm">IfcCableSegment</a></td><td>Cable segments may be aggregated into cable cores.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifccablesegmenttypeenum.htm">CORESEGMENT</a></td><td><a href="../../ifcelectricaldomain/lexical/ifccablesegment.htm">IfcCableSegment</a></td><td>Cable cores may be aggregated into cable conductors.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcCableSegment Object Aggregation</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td>Input</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The input end of the cable. While many cables may be bidirectional, port direction is indicated for connectivity purposes.</td></tr>
<tr><td>&nbsp;</td><td>Output</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">NOTDEFINED</a></td><td>The output end of the cable. While many cables may be bidirectional, port direction is indicated for connectivity purposes.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcCableSegment Port Nesting</p></td></tr></table>