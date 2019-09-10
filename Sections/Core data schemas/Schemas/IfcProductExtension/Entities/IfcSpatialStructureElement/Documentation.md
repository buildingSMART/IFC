A spatial structure element (_IfcSpatialStructureElement_) is the generalization of all spatial elements that might be used to define a spatial structure. That spatial structure is often used to provide a project structure to organize a building project.

A spatial project structure might define as many levels of decomposition as necessary for the building project. Elements within the spatial project structure are:

* site as _IfcSite_ 
* building as _IfcBuilding_ 
* storey as _IfcBuildingStorey_ 
* space as _IfcSpace_ 

or aggregations or parts thereof. The composition type declares an element to be either an element itself, or an aggregation (complex) or a decomposition (part). The interpretation of these types is given at each subtype of _IfcSpatialStructureElement_.

The _IfcRelAggregates_ is defined as an 1-to-many relationship and used to establish the relationship between exactly two levels within the spatial project structure. Finally the highest level of the spatial structure is assigned to _IfcProject_ using the _IfcRelAggregates_.

**Informal proposition**:

1. The spatial project structure, established by the _IfcRelAggregates_, shall be acyclic. 
2. A site should not be (directly or indirectly) associated to a building, storey or space. 
3. A building should not be (directly or indirectly) associated to a storey or space. 
4. A storey should not be (directly or indirectly) associated to a space. 

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
        Release 2x.</font>
> 


****Spatial Structure Use Definition****

<table cellpadding="2" cellspacing="2" summary="spatial structure">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <img src="figures/ifcspatialstructureelement-spatialstructure.png" alt="fig1" border="0" height="701" width="551">
          </td>
          <td align="left" valign="top">
            <p><small>The figure shows the use of <i>IfcRelAggregates</i>
            to establish a spatial structure including site,
            building, building section and storey. More
            information is provided at the level of the subtypes.</small></p>
          </td>
        </tr>
      </tbody>
    </table>