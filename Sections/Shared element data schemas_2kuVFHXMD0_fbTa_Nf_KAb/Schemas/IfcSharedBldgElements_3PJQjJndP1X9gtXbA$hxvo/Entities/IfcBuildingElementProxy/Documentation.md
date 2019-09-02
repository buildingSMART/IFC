The _IfcBuildingElementProxy_ is a proxy definition that provides the same functionality as subtypes of _IfcBuildingElement_, but without having a predefined meaning of the special type of building element, it represents.

Proxies can also be used as spatial place holders or provisions, that maybe later replaced by special types of elements.

One use of the proxy object is a provision for voids, i.e. where a particular volume of space is requested by some engineering function that might later be accepted or rejected and if accepted potentially transformed into a void within a building element, like a wall opening, or a slab opening. The provision for voids is exchanged as an _IfcBuildingElementProxy_ with the _PredefinedType_ = ProvisionForVoid.

Other usages of _IfcBuildingElementProxy_ include:

* The _IfcBuildingElementProxy_ can be used to exchange special types of building elements for which the current specification does not yet provide a semantic definition.
* The _IfcBuildingElementProxy_ can also be used to represent building elements for which the participating applications can not provide a semantic definition.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _CompositionType_ has been replaced by _PredefinedType_, being a superset of the enumerators.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcBuildingElement_: [Product Assignment](../../templates/product-assignment.htm), [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcbuildingelementproxy.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcsharedbldgelements/lexical/ifcbuildingelementproxytype.htm">IfcBuildingElementProxyType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcBuildingElementProxy Object Typing</p></td></tr></table>

> NOTE&nbsp; The _IfcBuildingElementProxyType_ can be used to share common information among many occurrences of the same proxy without establishing a particular semantic meaning of the type.

If no _IfcBuildingElementProxyType_ is attached (i.e. if only occurrence information is available) the _PredefinedType_ should be provided. If set to .USERDEFINED. a user defined value has to be provided by the _ObjectType_ attribute.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgelements/Pset_BuildingElementProxyCommon.xml">Pset_BuildingElementProxyCommon</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedbldgelements/Pset_BuildingElementProxyProvisionForVoid.xml">Pset_BuildingElementProxyProvisionForVoid</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_ConcreteElementGeneral.xml">Pset_ConcreteElementGeneral</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementFabrication.xml">Pset_PrecastConcreteElementFabrication</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementGeneral.xml">Pset_PrecastConcreteElementGeneral</a></td></tr>
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
<tr><td><p class="table">Table 2 &mdash; IfcBuildingElementProxy Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Material Single

The [Material Single](../../templates/material-single.htm) concept applies to this entity.

The material of the _IfcBuildingElementProxy_ is defined by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcBuildingElementProxy_ with the _PredefinedType_ = ProvisionForVoid.

Material information can also be given at the _IfcBuildingElementProxyType_, defining the common attribute data for all occurrences of the same type.&nbsp;It is then accessible by the inverse _IsTypedBy_ relationship pointing to _IfcBuildingElementProxyType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_ to _IfcMaterial_. If both are given, then the material directly assigned to _IfcBuildingElementProxy_ overrides the material assigned to _IfcBuildingElementProxyType_.

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Default spatial container </td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td><td>Spatial container for the element if it cannot be assigned to a building storey</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcsite.htm">IfcSite</a></td><td>Spatial container for the element in case that it is placed on site (outside of building)</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcBuildingElementProxy Spatial Containment</p></td></tr></table>

The _IfcBuildingElementProxy_, as any subtype of _IfcBuildingElement_, may participate alternatively in one of the two different containment relationships:

* the _Spatial Containment_ (defined here), or
* the _Element Composition_.