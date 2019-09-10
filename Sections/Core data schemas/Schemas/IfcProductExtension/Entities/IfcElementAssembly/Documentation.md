A container class that represents complex element assemblies aggregated from several elements, such as discrete elements, building elements, or other elements.

> <small>EXAMPLE Steel construction assemblies, such as
        trusses and different kinds of frames, can be represented
        by the <i>IfcElementAssembly</i> entity. Other examples
        include slab fields aggregated from a number of precast
        concrete slabs or reinforcement units made from several
        reinforcement bars.</small>
> 


> <font color="#0000FF"><small>HISTORY New Entity for
        Release IFC2x Edition 2.</small></font>
> 


****Containment Use Definition****

The _IfcElementAssembly_ should have (and in most implementation scenarios it is mandatory) a relationship for its hierarchical containment in the spatial structure of the project.

* The _IfcElementAssembly_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of _IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container. 

The _IfcElementAssembly_ shall represent an aggregate, i.e. it should have other elements, being subtypes of _IfcElement_, as contained (sub)parts.

* The _IfcElementAssembly_ is an aggregate i.e. being composed by other elements and acting as an assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.IsDecomposedBy_. Components of an assembly are described by instances of subtypes of _IfcElement_. 
* In this case, the contained subtypes of _IfcElement_ shall not be additionally contained in the project spatial hierarchy, i.e. the inverse attribute _SELF\IfcElement.ContainedInStructure_ of those _IfcElement_'s shall be _NIL._ 

<table border="0" cellpadding="2" cellspacing="2" summary="containment">
      <tr>
        <td>
          <img src="figures/ifcelementassembly-containment.png" alt="containment relationships" width="501" height="250" border="0">
        </td>
        <td valign="bottom">
          <p>
            <small>FIGURE spatial containment and element
            aggregation relationships for
            <i>IfcElementAssembly</i></small>
          </p>
        </td>
      </tr>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcElementAssembly_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcElementAssembly_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

****Geometric Representations****

The geometry of an _IfcElementAssembly_ is generally formed from its components, in which case it does not need to have an explicit geometric representation. In some cases it may be useful to also expose a simple explicit representation as a bounding box representation of the complex composed shape independently.

**Informal proposition**

1. The _IfcElementAssembly_ shall have an aggregation relationship to the contained parts, i.e. the (INV) _IsDecomposedBy_ relationship shall be utilized.