An element component is a representation for minor items included in, added to or connecting to or between elements, which usually are not of interest from the overall building structure viewpoint. However, these small parts may have vital and load carrying functions within the construction. These items do not provide any actual space boundaries. Typical examples of _IfcElementComponent_s include different kinds of fasteners and various accessories.

One or several instances of subtypes of _IfcElementComponent_ should always be accompanied by a defining instance of a respective subtype of _IfcElementComponentType_. The type object holds shape and material information.

> HISTORY&nbsp; New entity in IFC2x2

It is often desirable to model a number of same-shaped element components by means of a single occurrence object, e.g. several bolts within a connection or a row of reinforcement elements. In this IFC release, this is possible by means of multiple mapped representation as documented below.

To express the multiplicity of element components also on a higher semantic level, a _Qto_ElementComponentPatternQuantities_ should be provided via _IfcRelDefinesByProperties_ and contain the number of pieces which are placed by a single _IfcElementComponent_ instance.

{ .use-head}
**Symbolic Representation**

A symbolic representation is defined for a row of components or several rows of components within a single instance of _IfcElementComponent_. Such rows or arrays may contain possibly large numbers of individual pieces. The product definition shape consists of an _IfcShapeRepresentation_ with the attribute values

* _RepresentationIdentifier_ : 'Row'
* _RepresentationType_ : 'GeometricCurveSet'

and one or several curves as geometric items. The curves represent where reference points of the pieces are located. For example, such reference points may be at the heads of mechanical fasteners or at the starting point of the extrusion axis of reinforcement bars. In case of straight components (bolts, nails, staples, straight reinforcement bars, or similar), the local placement of the _IfcElementComponent_ shall be located and oriented such that the local z axis is parallel with the axes of the components. A _Qto_ElementComponentPatternQuantities_ should denote the count of pieces in the row or array and their spacing.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcelementcomponent.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
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
<tr><td><p class="table">Table 1 &mdash; IfcElementComponent Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Mapped Geometry

The [Mapped Geometry](../../templates/mapped-geometry.htm) concept applies to this entity.

The mapped item, _IfcMappedItem_, should be used if appropriate as it allows for reusing the geometry definition of a type at all occurrences of the same type.

A single instance of a subtype of _IfcElementComponent_ can stand for several actual element components at once. In this case, the _IfcShapeRepresentation_ contains as many mapped items as there are element components combined within this occurrence object.

&nbsp;

<table>

 <tr>
  <td><img src="../../../figures/ifcelementcomponent_multiple.png"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates multiple components modeled as a single occurrence object (here: <em>IfcFastener</em>)</blockquote></td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Element component mapped representation</p></td>
  <td><p>&nbsp;</p></td>
 </tr>

</table>

Representation identifier and type are the same as in single mapped representation. The number of mapped items in the representation corresponds with the count of element components in the _IfcElementQuantity_.