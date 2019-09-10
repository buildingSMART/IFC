The element type _IfcDistributionFlowElementType_ defines a list of commonly shared property set definitions of an element and an optional set of product representations. It is used to define an element specification (the specific product information that is common to all occurrences of that product type).

Distribution flow element types (orthe instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcDistributionFlowElementType_ are represented by instances of _IfcDistributionFlowElement_ or its subtypes.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Ports may now be defined using _IfcRelNests_ to enable definition of ports at type definitions (both forward and backward compatible), provide a logical order, and reduce the number of relationship objects needed. The relationship _IfcRelConnectsPortToElement_ is still supported on occurrence objects, however is now specific to dynamically connected ports.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcdistributionflowelementtype.htm)

{ .use-head}
Type Axis Geometry

The [Type Axis Geometry](../../templates/type-axis-geometry.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Geometry</b></th></tr>
<tr><td>Curve3D</td><td><a href="../../ifcgeometryresource/lexical/ifcboundedcurve.htm">IfcBoundedCurve</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDistributionFlowElementType Type Axis Geometry</p></td></tr></table>

This represents the 3D flow path of the item having _IfcShapeRepresentation.RepresentationType_ of 'Curve3D' and containing a single _IfcBoundedCurve_ subtype such as _IfcPolyline_, _IfcTrimmedCurve_, or _IfcCompositeCurve_. For elements containing directional ports (_IfcDistributionPort_ with _FlowDirection_ of _SOURCE_ or _SINK_), the direction of the curve indicates direction of flow where a _SINK_ port is positioned at the start of the curve and a _SOURCE_ port is positioned at the end of the curve. This representation is most applicable to flow segment types (pipes, ducts, cables), however may be used at other elements to define a primary flow path if applicable.

If an element type is defined parametrically (such as a flow segment type defining common material profile but no particular length or path), then no representations shall be asserted at the type.

> NOTE&nbsp; The product representations are defined as representation maps (at the level of the supertype _IfcTypeProduct_, which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[1]_ being an _IfcMappedItem_.

  
  
{ .use-head}
Type Clearance Geometry

The [Type Clearance Geometry](../../templates/type-clearance-geometry.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Geometry</b></th></tr>
<tr><td>Surface3D</td><td><a href="../../ifcgeometryresource/lexical/ifcsurface.htm">IfcSurface</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcDistributionFlowElementType Type Clearance Geometry</p></td></tr></table>

This represents the 3D clearance volume of the item having _RepresentationType_ of 'Surface3D'. Such clearance region indicates space that should not intersect with the 'Body' representation between element occurrences, though may intersect with the 'Clearance' representation of other element occurrences. The particular use of clearance space may be for safety, maintenance, or other purposes.

  
  
{ .use-head}
Type Lighting Geometry

The [Type Lighting Geometry](../../templates/type-lighting-geometry.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Geometry</b></th></tr>
<tr><td>LightSource</td><td><a href="../../ifcpresentationorganizationresource/lexical/ifclightsource.htm">IfcLightSource</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcDistributionFlowElementType Type Lighting Geometry</p></td></tr></table>

This represents the light emission of the item having _IfcShapeRepresentation.RepresentationType_ of 'LightSource' and containing one or more _IfcLightSource_ subtypes. This representation is most applicable to lamps and light fixtures, however may be used at other elements that emit light.
