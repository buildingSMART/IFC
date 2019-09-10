A junction box is an enclosure within which cables are connected.

Cables may be members of an electrical circuit (for electrical power systems) or be information carriers (in a telecommunications system). A junction box is typically intended to conceal a cable junction from sight, eliminate tampering or provide a safe place for electrical connection.

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

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcjunctionbox.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtype.htm">IfcJunctionBoxType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcJunctionBox Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcelectricaldomain/Pset_JunctionBoxTypeCommon.xml">Pset_JunctionBoxTypeCommon</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcJunctionBox Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcelectricaldomain/Qto_JunctionBoxBaseQuantities.xml">Qto_JunctionBoxBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcJunctionBox Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Casing</td><td>Material from which the casing is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcJunctionBox Material Constituents</p></td></tr></table>

  
  
{ .use-head}
Element Connectivity

The [Element Connectivity](../../templates/element-connectivity.htm) concept applies to this entity as shown in Table 5.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcsharedcomponentelements/lexical/ifcdiscreteaccessory.htm">IfcDiscreteAccessory</a></td><td>Indicates a cover plate for the junction box, having ObjectType 'JunctionBoxCoverPlate'.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 5 &mdash; IfcJunctionBox Element Connectivity</p></td></tr></table>

  
  
{ .use-head}
Element Filling

The [Element Filling](../../templates/element-filling.htm) concept applies to this entity as shown in Table 6.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td>IfcCovering</td><td>Covering such as drywall applied to a wall or ceiling, for which the junction box fills.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 6 &mdash; IfcJunctionBox Element Filling</p></td></tr></table>

  
  
{ .use-head}
Port Nesting

The [Port Nesting](../../templates/port-nesting.htm) concept applies to this entity as shown in Table 7.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th><th><b>Flow</b></th><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">DATA</a></td><td>Line#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DATA</a></td><td>A data line, typically a cable connecting from a network router communications device.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">DATA</a></td><td>Line#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DATA</a></td><td>A data line, typically a cable connecting from a network router communications device.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">DATA</a></td><td>Gang#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DATA</a></td><td>A slot to house a data outlet containing one or more jacks, ordered from left-to-right.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">DATA</a></td><td>Gang#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">DATA</a></td><td>A slot to house a data outlet containing one or more jacks, ordered from left-to-right.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Line</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SINK</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The electrical supply line, typically a cable connecting from another junction box or from a protective device within a distribution board.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Load</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>The next load in the circuit, typically a cable connecting to another junction box.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Gang#1</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>A slot to house a switch or outlet, ordered from left-to-right.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Gang#2</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>A slot to house a switch or outlet, ordered from left-to-right.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Gang#3</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>A slot to house a switch or outlet, ordered from left-to-right.</td></tr>
<tr><td><a href="../../ifcelectricaldomain/lexical/ifcjunctionboxtypeenum.htm">POWER</a></td><td>Gang#4</td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcflowdirectionenum.htm">SOURCE</a></td><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystemenum.htm">ELECTRICAL</a></td><td>A slot to house a switch or outlet, ordered from left-to-right.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 7 &mdash; IfcJunctionBox Port Nesting</p></td></tr></table>
