A transport element is a generalization of all transport related objects that move people, animals or goods within a building or building complex. The _IfcTransportElement_ defines the occurrence of a transport element, that (if given), is expressed by the _IfcTransportElementType_.

> EXAMPLE&nbsp; Transportation elements include elevator (lift), escalator, moving walkway, etc.

> NOTE&nbsp; More detailed equipment that may be a part of a transportation device, like a lifting hook, is defined as _IfcDiscreteAccessory_. It maybe included as a part of the _IfcTransportElement_ by virtue of the objectified relationship _IfcRelAggregates_.

Depending on local classification systems transport elements and transportation systems in buildings are either considered as part of a building system, or as part of a building service system. Within IFC they are considered as part of a building system and may have to be mapped appropriately.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x}
> IFC2x CHANGE&nbsp; The attribute _PredefinedType_ (previously OperationType) is made optional.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The last attributes CapacityByWeight and CapacityByNumber are removed, use Pset_TransportElementCommon instead.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifctransportelement.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity.

_IfcTransportElement_ defines the occuurence of any transportation device, common information about transportation device types (or styles) is handled by _IfcTransportElementType_. The _IfcTransportElementType_ (if present) may establish the common&nbsp;type name, usage (or predefined) type, common material layer set, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcTransportElementType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _<font color="#0000FF">IsTypedBy</font>_ attribute.

If no _IfcTransportElementType_ is attached&nbsp;(i.e. if only occurrence information is given) the _PredefinedType_ should be provided. If set to .USERDEFINED. a user defined value can be provided by the _ObjectType_ attribute.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_TransportElementCommon.xml">Pset_TransportElementCommon</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifctransportelementtypeenum.htm">ELEVATOR</a></td><td><a href="../../psd/ifcproductextension/Pset_TransportElementElevator.xml">Pset_TransportElementElevator</a></td></tr>
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
<tr><td><p class="table">Table 1 &mdash; IfcTransportElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity.

* The _IfcTransportElement_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, refering to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuilding_ being the default container.
