Layers or major components as subordinate parts of a building element. Typical usage examples include precast concrete sandwich walls, where the layers may have different geometry representations. In this case the layered material representation does not sufficiently describe the element. Each layer is represented by an own instance of the _IfcBuildingElementPart_ with its own geometry description.

> <font color="#0000ff" size="-1">
HISTORY New entity in IFC
Release 2x2 </font>

**General usage**

The exact type information of the _IfcBuildingElementPart_ is given in the _ObjectType_ attribute inherited from _IfcObject_. Standard type designations are provided for guideline below. Other object type values may be defined in local agreements.

<table border="1">
  <tbody>
    <tr>
      <td><i><b>Standard building element part type
designation</b></i></td>
      <td><i><b>Description</b></i></td>
    </tr>
    <tr>
      <td>'Insulation layer'</td>
      <td>The part consists of an insulation layer, for example
as thermal
isolation between wall panels in sandwich walls. </td>
    </tr>
    <tr>
      <td>'Precast panel'</td>
      <td>The part is a precast panel, usually as an internal or
external
layer in a sandwich wall panel.</td>
    </tr>
    <tr>
      <td>'Wooden part'</td>
      <td>A wooden part included or embedded in a building
element.</td>
    </tr>
  </tbody>
</table>

****Property Set Use Definition****:

The property sets relating to the _IfcBuildingElementPart_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcBuildingElementPart_ are part of this IFC release:

* [Pset_ConcreteElementSurfaceFinishQuantityGeneral](../../psd/IfcStructuralElementsDomain/Pset_ConcreteElementSurfaceFinishQuantityGeneral.xml){ target="SOURCE"}: common property set for all _IfcBuildingElementPart_ occurrences related to concrete construction. (Note: this is a general property set, which relates to many IFC classes, e.g. subtypes of _IfcBuildingElement_). 
* [Pset_PrecastConcreteElementGeneral](../../psd/IfcStructuralElementsDomain/Pset_PrecastConcreteElementGeneral.xml){ target="SOURCE"}: common property set for all _IfcBuildingElementPart_ occurrences related to precast concrete construction. (Note: this is a general property set, which relates to many IFC classes, e.g. subtypes of _IfcBuildingElement_). 

**Geometry Use Definitions:**

The geometric representation of _IfcBuildingElementPart_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The use of local placement is defined at the supertype _IfcBuildingElementComponent_.

**Standard Geometric Representation**  
The use of Standard Geometric Representations is defined at the supertype _IfcBuildingElementComponent_.