The _IfcElementAssembly_ represents complex element assemblies aggregated from several elements, such as discrete elements, building elements, or other elements.

> EXAMPLE Steel construction assemblies, such as trusses and different kinds of frames, can be represented by the _IfcElementAssembly_ entity. Other examples include slab fields aggregated from a number of precast concrete slabs or reinforcement units made from several reinforcement bars. Also bathroom units, staircase sections and other premanufactured or precast elements are examples of the general _IfcElementAssembly_ entity

> NOTE&nbsp; The _IfcElementAssembly_ is a general purpose entity that is required to be decomposed. Also other subtypes of IfcElement can be decomposed, with some dedicated entities such as _IfcWallElementedCase_ and _IfcSlabElementedCase_.

The assembly structure can be nested, i.e. an _IfcElementAssembly_ could be an aggregated part within another _IfcElementAssembly_.

> NOTE&nbsp; View definitions and/or implementer agreements may restrict the number of allowed levels of nesting.

The geometry of an _IfcElementAssembly_ is generally formed from its components, in which case it does not need to have an explicit geometric representation. In some cases it may be useful to also expose an own explicit representation of the aggregate.

> NOTE&nbsp; View definitions or implementer agreements may further constrain the applicability of certain shape representations at the _IfcElementAssembly_ in respect of the shape representations of its parts.

> HISTORY&nbsp; New entity in IFC2x2.

{ .spec-head}
Informal Propositions:

1. The _IfcElementAssembly_ shall have an aggregation relationship to the contained parts, i.e. the (INV) _IsDecomposedBy_ relationship shall be utilzed.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcelementassembly.htm)

{ .use-head}
Object Typing

The [Object Typing](../../templates/object-typing.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcelementassemblytype.htm">IfcElementAssemblyType</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcElementAssembly Object Typing</p></td></tr></table>

  
  
{ .use-head}
Object Aggregation

The [Object Aggregation](../../templates/object-aggregation.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>RelatedObjects</b></th><th><b>Description</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcmember.htm">IfcMember</a></td><td>Members within the assembly.</td></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedbldgelements/lexical/ifcplate.htm">IfcPlate</a></td><td>Plates within the assembly.</td></tr>
<tr><td>&nbsp;</td><td><a href="../../ifcsharedcomponentelements/lexical/ifcelementcomponent.htm">IfcElementComponent</a></td><td>Components within the assembly.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcElementAssembly Object Aggregation</p></td></tr></table>

The _IfcElementAssembly_ shall represent an aggregate, i.e. it should have other elements, being subtypes of _IfcElement_, as contained (sub)parts. The table above only represents a selection of subtypes of _IfcElement_ that are legitimate as parts in an _IfcElementAssembly_

* The _IfcElementAssembly_ is an aggregate i.e. being composed by other elements and acting as an assembly using the objectified relationship _IfcRelAggregates_, refering to it by its inverse attribute _SELF\IfcObjectDefinition.IsDecomposedBy_. Components of an assembly are described by instances of subtypes of _IfcElement_.
* In this case, the contained subtypes of _IfcElement_ shall not be additionally contained in the project spatial hierarchy, i.e. the inverse attribute _SELF\IfcElement.ContainedInStructure_ of those _IfcElement_'s shall be _NIL._

Figure 1 illustrates spatial containment and element aggregation relationships.

!["containment relationships"](../../../figures/IfcElementAssembly-Containment.png "Figure 1 &mdash; Element assembly containment")

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td><td>Default spatial container</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td><td>Spatial container for element assemblies not assignable to a building storey</td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcsite.htm">IfcSite</a></td><td>Spatial container for element assemblies that are placed on site (outside of building)</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcElementAssembly Spatial Containment</p></td></tr></table>

The _IfcElementAssembly_ should have a relationship for its containment in the hierachical spatial structure of the project. Only if the _IfcElementAssembly_ is itself a part of another assembly this relationship should be omitted.