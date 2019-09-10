A feature element is a generalization of all existence dependent elements which modify the shape and appearance of the associated master element. The _IfcFeatureElement_ offers the ability to handle shape modifiers as semantic objects within the IFC object model.

> NOTE&nbsp; The term "feature" has a predefined meaning in a context of "feature-based modeling" and within steel construction work. It is introduced here in a broader sense to cover all existence dependent, but semantically described, modifiers of an element's shape and appearance. It is envisioned that future releases enhance the feature-based capabilities of the IFC model.

In contrary to the aggregation, as used in _IfcElementAssembly_, that defines the aggregate as a container element, that has equally treated parts, the feature concept introduced by _IfcFeatureElement_ defines the master element with subordinate parts as additions, or with voids or cut-outs as subtractions.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x2}
> IFC2x2 CHANGE&nbsp; The entity is introduced as an upward compatible extension of the IFC2x platform. It is an intermediate abstract supertype without defining its own explicit attributes.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcfeatureelement.htm)

{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity.

As a subordinate part being fully dependent on the master element the _IfcFeatureElement_ shall have no independent containment relationship to the spatial structure.

* The _SELF\IfcElement.ContainedInStructure_ relationship shall be NIL.