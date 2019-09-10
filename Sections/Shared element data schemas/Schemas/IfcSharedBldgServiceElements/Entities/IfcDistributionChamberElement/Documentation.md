A distribution chamber element defines a place at which distribution systems and their constituent elements may be inspected or through which they may travel.

An **IfcDistributionChamberElement** is a formed volume used in a distribution system, such as a sump, trench or manhole. Instances of [IfcDistributionSystem](../../ifcsharedbldgserviceelements/lexical/ifcdistributionsystem.htm) or [IfcDistributionFlowElement](../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelement.htm) may be related to the **IfcDistributionChamberElement** enabling their location in or at the chamber to be determined.

> HISTORY&nbsp; New entity in IFC2x2.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionFlowElement_: [Axis Geometry](../../templates/axis-geometry.htm), [Clearance Geometry](../../templates/clearance-geometry.htm), [Lighting Geometry](../../templates/lighting-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcdistributionchamberelement.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtype.htm">IfcDistributionChamberElementType</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionflowelementtype.htm">IfcDistributionFlowElementType</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDistributionChamberElement Object Typing</p></td></tr></table>

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementCommon.xml">Pset_DistributionChamberElementCommon</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">FORMEDDUCT</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeFormedDuct.xml">Pset_DistributionChamberElementTypeFormedDuct</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">INSPECTIONCHAMBER</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeInspectionChamber.xml">Pset_DistributionChamberElementTypeInspectionChamber</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">INSPECTIONPIT</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeInspectionPit.xml">Pset_DistributionChamberElementTypeInspectionPit</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">MANHOLE</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeManhole.xml">Pset_DistributionChamberElementTypeManhole</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">METERCHAMBER</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeMeterChamber.xml">Pset_DistributionChamberElementTypeMeterChamber</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">SUMP</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeSump.xml">Pset_DistributionChamberElementTypeSump</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">TRENCH</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeTrench.xml">Pset_DistributionChamberElementTypeTrench</a></td></tr>
<tr><td><a href="../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtypeenum.htm">VALVECHAMBER</a></td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_DistributionChamberElementTypeValveChamber.xml">Pset_DistributionChamberElementTypeValveChamber</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcDistributionChamberElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th></tr>
<tr><td><a href="../../qto/ifcsharedbldgserviceelements/Qto_DistributionChamberElementBaseQuantities.xml">Qto_DistributionChamberElementBaseQuantities</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcDistributionChamberElement Quantity Sets</p></td></tr></table>

  
  
{ .use-head}
Material Constituents

The [Material Constituents](../../templates/material-constituents.htm) concept applies to this entity as shown in Table 4.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Name</b></th><th><b>Description</b></th></tr>
<tr><td>Base</td><td>The material from which the base of the duct is constructed.</td></tr>
<tr><td>Cover</td><td>The material from which the access cover to the chamber is constructed.</td></tr>
<tr><td>Fill</td><td>The material that is  used to fill the duct (where used).</td></tr>
<tr><td>Wall</td><td>The material from which the wall of the duct is constructed.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 4 &mdash; IfcDistributionChamberElement Material Constituents</p></td></tr></table>

The material of the **IfcDistributionChamberElement** is defined by [IfcMaterialConstituentSet](../../ifcmaterialresource/lexical/ifcmaterialconstituentset.htm) or as a fallback by [IfcMaterial](../../ifcmaterialresource/lexical/ifcmaterial.htm), and attached by the _RelatingMaterial_ attribute on the [IfcRelAssociatesMaterial](../../ifcproductextension/lexical/ifcrelassociatesmaterial.htm) relationship. It is accessible by the _HasAssociations_ inverse attribute. Material information can also be given at the [IfcDistributionChamberElementType](../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtype.htm), defining the common attribute data for all occurrences of the same type. The following keywords for _IfcMaterialConstituentSet.MaterialConstituents[n].Name_ shall be used:

* **'Base'**: The material from which the base of the duct is constructed.
* **'Cover'**: The material from which the access cover to the chamber is constructed.
* **'Fill'**: The material that is used to fill the duct (where used).
* **'Wall'**: The material from which the wall of the duct is constructed.