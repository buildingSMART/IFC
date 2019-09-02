The _RepresentationMaps_ define the type product shape and multiple geometric representations can be assigned. If a product occurrence is assigned to the type by using the _IfcRelDefinesByType_ relationship, then these occurrences have to reference the representation maps. The reference is created by one or multiple _IfcShapeRepresentation_'s having an _IfcMappedItem_ as _Items_, that places the _IfcRepresentationMap_ of the type product into the spatial contexts, i.e. by using an Cartesian transformation operator to transform the _IfcRepresentationMap_ into the object coordinate system of the product occurrence.

Figure 1 illustrates an example of referencing a representation map by the shape representation of a product occurrence. Here the Cartesian transformation operator only uses translation, but no rotation, mirroring, or scaling.

!["representation map"](../../../figures/ifctypeproduct_representationmap-1.png "Figure 1 &mdash; Product type geometry with single placement")

Figure 2 illustrates an example of referencing a representation multiple times map by the shape representation of a product occurrence. Here the Cartesian transformation operator only uses translation, but no rotation, mirroring, or scaling. The different translation values determine the pattern of the multiple placement.

!["representation map"](../../../figures/ifctypeproduct_representationmap-2.png "Figure 2 &mdash; Product type geometry with multiple placement")