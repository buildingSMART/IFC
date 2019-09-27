﻿_IfcShapeAspect_ allows for grouping of shape representation items that represent aspects (or components) of the shape of a product. Thereby shape representations of components of the product shape represent a distinctive part to a product that can be explicitly addressed.

The _IfcShapeAspect_'s may have distinct material information or other distict characteristics that differs from other parts of the product shape representation.

> NOTE&nbsp; The _IfcShapeAspect_ together with the _IfcMaterialConstituent_ can be used to associate distict material information to parts of the product shape representation.

Figure 1 indicates the association of material characteristics to shape aspects.

!["shape"](../../../../../../figures/ifcshapeaspect_fig1.png "Figure 1 &mdash; shape aspects for associating material")

{ .extDef}
> NOTE&nbsp; Definition from ISO 10303-41:  
> A shape aspect is an identifiable element of the shape of an object.

> NOTE&nbsp; Entity adapted from **shape_aspect** defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC2.0

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Attribute _PartOfProductDefinitionShape_ declared OPTIONAL and extended to type _IfcProductRepresentationSelect_ with upward compatibility for file based exchange.

{ .spec-head}
Informal Propositions:

1. If _ShapeRepresentations_ points to shape representations that are part of an _IfcProductDefinitionShape_, _PartOfProductDefinitionShape_ must refer to this instance of _IfcProductDefinitionShape_.
2. If _ShapeRepresentations_ points to shape representations that are part of an _IfcRepresentationMap_, _PartOfProductDefinitionShape_ must refer to this instance of _IfcRepresentationMap_.
