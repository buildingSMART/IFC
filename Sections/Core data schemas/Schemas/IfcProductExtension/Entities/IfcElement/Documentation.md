Generalization of all components that make up an AEC product. Those elements can be logically contained by a spatial structure element that constitutes a certain level within a project structure hierarchy (e.g., site, building, storey or space). This is done by using the _IfcRelContainedInSpatialStructure_ relationship.

Elements are physically existent objects, although they might be void elements, such as holes. Elements either remain permanently in the AEC product, or only temporarily, as formwork does. Elements can be either assembled on site or pre-manufactured and built in on site.

> <font size="-1">EXAMPLEs of elements in a building
      construction context are walls, floors, windows and
      recesses.</font>

An element can have material and quantity information assigned through the _IfcRelAssociatesMaterial_ and _IfcRelDefinesByProperties_ relationship.

In addition an element can be declared to be a specific occurrence of an element type (and thereby be defined by the element type properties) using the _IfcRelDefinesByType_ relationship.

An element can also be defined as an element assembly that is a group of semantically and topologically related elements that form a higher level part of the AEC product. Those element assemblies are defined by virtue of the _IfcRelAggregates_ relationship.

> <font size="-1">EXAMPLEs for element assembly are complete
      Roof Structures, made by several Roof Areas, or a Stair,
      composed by Flights and Landings.</font>

Elements that performs the same function may be grouped by an "Element Group By Function". It is realized by an instance of _IfcGroup_ with the _ObjectType_ = 'ElementGroupByFunction".

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
        Release 1.0</font>
> 


****Property Set Use Definition****:

The property sets relating to the _IfcElement_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcElement_ are part of this IFC release:

<ul>
      <li>
        <a href="../../psd/IfcProductExtension/Pset_Draughting.xml" target="SOURCE">Pset_Draughting</a>: common property set
        for elements introduced to handle the assignment of CAD
        related information (here layer name and object colour).
        <ul>
          <li>
            <font color="#FF0000"><small>IFC2x3 CHANGE  The use
            of this property set is deprecated from IFC2x3
            onwards, curve colours are handled by
            <i>IfcCurveStyle</i>, and layer assignment are
            handled by
            <i>IfcPresentationLayerAssignment</i>.</small></font>
          </li>
        </ul>
      </li>
      <li>
        <a href="../../psd/IfcProductExtension/Pset_QuantityTakeOff.xml" target="SOURCE">Pset_QuantityTakeOff</a>: common property
        set for elements introduced to handle additional
        description of quantity take off.
      </li>
      <li>
        <a href="../../psd/IfcProductExtension/Pset_ElementShading.xml" target="SOURCE">Pset_ElementShading</a>: common property
        set for elements that have shading properties to be used
        in energy calculations or simulations
      </li>
    </ul>
****Quantity Use Definition****:

The quantities relating to the _IfcElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. A detailed specification for individual quantities is introduced at the level of subtypes of _IfcElement_.

****Geometry Use Definitions****

The geometric representation of any _IfcElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations. A detailed specification for the shape representation is introduced at the level of subtypes of _IfcElement_.
