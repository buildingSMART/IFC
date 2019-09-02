This entity is a generalization of all elements that participate in a distribution system. Typical examples of _IfcDistributionElement_ are (among others):

* building service elements within a heating systems 
* building service elements within a cooling system 
* building service elements within a ventilation system 
* building service elements within a plumbing system 
* electrical elements 
* elements within a communication network 

The _IfcDistributionElement_ is further specialized in the IFC model. Direct instantiation of _IfcDistributionElement_ without an assigned subtype of _IfcDistributionElementType_ provides the meaning of an distribution element proxy.

> HISTORY&nbsp; New entity in IFC1.5.

{ .change-ifc2x4}
> IFC4 CHANGE The entity is marked as deprecated for instantiation - will be made ABSTRACT in future releases.

&nbsp;

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcdistributionelement.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcdistributionelementtype.htm">IfcDistributionElementType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDistributionElement Object Typing</p></td></tr></table>

The _IfcDistributionElement_ defines the occurrence of any HVAC, electrical, sanitary or other element within a distribution system. Common information about distribution element types (or styles) is handled by subtypes of _IfcDistributionElementType_. The _IfcDistributionElementType_ (if present) may establish the common type name, usage (or predefined) type, common material, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcDistributionElementType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

The assignment of types to distribution element occurrences is vital for providing the additional meaning, or ontology, of the distribution element. Many specialized type are defined in other schemas of this specification.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcDistributionElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Quantity Sets

The [Quantity Sets](../../templates/quantity-sets.htm) concept applies to this entity.

The quantities relating to the _IfcDistributionElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. A detailed specification for individual quantities is introduced at the level of subtypes of _IfcDistributionElement_.

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcDistributionElement Spatial Containment</p></td></tr></table>

The _IfcDistributionElement_ may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second (optional) relationship is the aggregation within an&nbsp;element assembly.

* The _IfcDistributionElement_ is places within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcSpace_ being the default container. 
* The _IfcDistributionElement_ may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype. In this case it should not be additionally contained in the project spatial hierarchy, i.e.&nbsp;_SELF\IfcElement.ContainedInStructure_ should be _NIL._