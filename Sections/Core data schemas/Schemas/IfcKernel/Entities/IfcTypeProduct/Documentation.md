_IfcTypeProduct_ defines a type definition of a product without being already inserted into a project structure (without having a placement), and not being included in the geometric representation context of the project. It is used to define a product specification, that is, the specific product information that is common to all occurrences of that product type.

An _IfcTypeProduct_ may have a list of property set attached and an optional set of product representations. Values of these properties and the representation maps are common to all occurrences of that product type. The type-occurrence relationship is realized using the objectified relationship _IfcRelDefinesByType_.

> NOTE&nbsp; The product representations are defined as representation maps, which may be assigned by a product instance through the representation item(s) being an _IfcShapeRepresentation_ and having _Items_ of type _IfcMappedItem_.

The representations at the occurrence level (represented by subtypes of _IfcProduct_) can override the specific representations at the type level:

* for geometric representations, a Cartesian transformation operator can be applied at the occurrence level.
* for property sets, a property within an occurrence property set, assigned at the product occurrence, overrides the same property assigned to the product type.

An _IfcTypeProduct_ may be exchanged without being already assigned to subtypes of _IfcProduct_.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The entity _IfcTypeProduct_ shall not be instantiated from IFC4 onwards. It will be changed into an ABSTRACT supertype in future releases of IFC.

{ .use-head}
Geometry use definition

The _RepresentationMaps_ define the type product shape and multiple geometric representations can be assigned. If a product occurrence is assigned to the type by using the _IfcRelDefinesByType_ relationship, then these occurrences have to reference the representation maps. The reference is created by one or multiple _IfcShapeRepresentation_'s having an _IfcMappedItem_ as _Items_, that places the _IfcRepresentationMap_ of the type product into the spatial contexts, i.e. by using an Cartesian transformation operator to transform the _IfcRepresentationMap_ into the object coordinate system of the product occurrence.

Figure 1 illustrates an example of referencing a representation map by the shape representation of a product occurrence. Here the Cartesian transformation operator only uses translation, but no rotation, mirroring, or scaling.

!["representation map"](../../../../../../figures/ifctypeproduct_representationmap-1.png "Figure 1 &mdash; Product type geometry with single placement")

Figure 2 illustrates an example of referencing a representation multiple times map by the shape representation of a product occurrence. Here the Cartesian transformation operator only uses translation, but no rotation, mirroring, or scaling. The different translation values determine the pattern of the multiple placement.

!["representation map"](../../../../../../figures/ifctypeproduct_representationmap-2.png "Figure 2 &mdash; Product type geometry with multiple placement")