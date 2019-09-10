A part of the foundation of a structure that spreads and transmits the load directly to the soil.

> <font color="#0000ff" size="-1">
HISTORY New entity in IFC
Release 2x2 </font>

****Property Set Use Definition****:

The property sets relating to the _IfcFooting_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcFooting_ are part of this IFC release:

* [Pset_ReinforcementBarCountOfIndependentFooting](../../psd/IfcStructuralElementsDomain/Pset_ReinforcementBarCountOfIndependentFooting.xml){ target="SOURCE"}: property set for independent _IfcFooting_ occurrences.
* [Pset_ReinforcementBarPitchOfContinuousFooting](../../psd/IfcStructuralElementsDomain/Pset_ReinforcementBarPitchOfContinuousFooting.xml){ target="SOURCE"}: property set for continuous _IfcFooting_ occurrences.

**Geometry Use Definitions:**

The geometric representation of _IfcFooting_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The local placement for _IfcFooting_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**Standard Geometric Representation**  
Provided that it is possible the standard geometric representation of _IfcFooting_ is defined using the swept solid representation. The _RepresentationType_ attribute of _IfcShapeRepresentation_ should have the value 'SweptSolid'. The following constraints apply to the standard representation:

* **Solid:** _IfcExtrudedAreaSolid_ shall be supported 
* **Profile:** All applicable profile types shall be supported 
* **Extrusion:** All extrusion directions shall be supported. 

If it is impossible to define the geometry using the swept solid representation the representations defined in its supertype _IfcBuildingElement_ may be used.