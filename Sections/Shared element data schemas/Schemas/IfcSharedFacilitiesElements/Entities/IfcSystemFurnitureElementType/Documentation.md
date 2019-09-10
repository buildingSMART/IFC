An _IfcSystemFurnitureElementType_ defines a particular type of component or element of systems or modular furniture.

> <font color="#0000ff" size="-1">HISTORY
New Entity in IFC 2x2 </font>

****Use Definitions****

An _IfcSystemFurnitureElementType_ provides for all types of elements of system furniture. Occurrences of a type of system furniture element are specified through _IfcFurnishingElement_. An occurrence of a complete _IfcFurnishingElement_ made up of system furniture elements is created using _IfcRelNests_ (if only the system furniture elements are specified) or _IfcRelAggregates_ (in cases where both the system furniture elements, means of joining together the elements and other accessories such as cable tray and wiring etc. are included).

****Property Set Use Definition****:

The property sets relating to an _IfcSystemFurnitureElementType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcSystemFurnitureElementType_ are part of this IFC release:

* [Pset_SystemFurnitureElementTypeCommon](../../psd/IfcSharedFacilitiesElements/Pset_SystemFurnitureElementTypeCommon.xml): property set for the properties common to all types of system furniture element, if available 
* [Pset_SystemFurnitureElementTypePanel](../../psd/IfcSharedFacilitiesElements/Pset_SystemFurnitureElementTypePanel.xml): specific property set for the properties of a system furniture panel, if available 
* [Pset_SystemFurnitureElementTypeWorkSurface](../../psd/IfcSharedFacilitiesElements/Pset_SystemFurnitureElementTypeWorkSurface.xml): specific property set for the properties of a system furniture work surface, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.

****Name Use Definitions****The name of the type of system furniture element is defined through the _IfcSystemFurnitureElementType.Name_ attribute (through inheritance from _IfcRoot_).

For further indormation on usage, refer to _IfcFurnitureType_
