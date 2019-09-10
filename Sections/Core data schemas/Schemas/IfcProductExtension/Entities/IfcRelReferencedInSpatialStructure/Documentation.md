This objectified relationship, _IfcRelReferencedInSpatialStructure_, is used to assign elements in addition to those levels of the project spatial structure, in which they are referenced, but not primarily contained.

> <small>NOTE  The primary containment relationship between
        an element and the spatial structure is handled
        by <i>IfcRelContainsInSpatialStructure</i>.</small>
> 


Any element can be referenced to zero, one or several levels of the spatial structure. Whereas the _IfcRelContainsInSpatialStructure_ relationship is required to be hierarchical (an element can only be contained in exactly one spatial structure element), the _IfcRelReferencedInSpatialStructure_ is not restricted to be hierarchical.

> <small>EXAMPLE A wall might be normally contained within
        a storey, and since it does not span through several
        stories, it is not referenced in any additional storey.
        However a curtain wall might span through several
        stories, in this case it can be contained within the
        ground floor, but it would be referenced by all
        additional stories, it spans.</small>
> 


Predefined spatial structure elements to which elements can be assigned are

* site as _IfcSite_ 
* building as _IfcBuilding_ 
* storey as _IfcBuildingStorey_ 
* space as _IfcSpace_ 

The same element can be assigned to different spatial structure elements depending on the context.

> <small><font color="#0000FF">HISTORY New entity
        in Release IFC2x Edition 3.</font></small>
> 


****Use Definition****

<table cellpadding="2" cellspacing="2" width="80%">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <img alt="reference and containment" src="figures/ifcrelreferencedinspatialstructure-fig1.png" height="601" width="601"><br>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <small>The figure shows the use of
            <i>IfcRelContainedInSpatialStructure</i> and
            IfcRelReferencedInSpatialStructure to assign an
            <i>IfcCurtainWall</i> to two different levels within
            the spatial structure. It is primarily contained
            within the ground floor, and additionally referenced
            within the first and second  floor.</small> 
          </td>
        </tr>
      </tbody>
    </table>
