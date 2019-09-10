**Definition from ISO 6707-1:1989**: Construction work that has the provision of shelter for its occupants or contents as one of its main purpose and is normally designed to stand permanently in one place.

A building represents a structure that provides shelter for its occupants or contents and stands in one place. The building is also used to provide a basic element within the spatial structure hierarchy for the components of a building project (together with site, storey, and space).

A building is (if specified) associated to a site. A building may span over several connected or disconnected buildings. Therefore building complex provides for a collection of buildings included in a site. A building can also be decomposed in (vertical) parts, where each part defines a building section. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElements_ which is interpreted as follow:

* COMPLEX = building complex 
* ELEMENT = building 
* PARTIAL = building section 

> <font color="#0000FF"><small>HISTORY New entity in
        IFC Release 1.0.</small></font>
> 


****Property Set Use Definition****:

The property sets relating to the _IfcBuilding_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcBuilding_ are part of this IFC release:

*  [Pset_BuildingCommon](../../psd/IfcProductExtension/Pset_BuildingCommon.xml){ target="SOURCE"}: common property set for all types of buildings 
*  [Pset_BuildingWaterStorage](../../psd/IfcProductExtension/Pset_BuildingWaterStorage.xml){ target="SOURCE"}: specific property set for buildings to capture the water supply requirements 
*  [Pset_BuildingUse](../../psd/IfcProductExtension/Pset_BuildingUse.xml){ target="SOURCE"}: specific property set for buildings to capture the current and anticipated real estate context. 
*  [Pset_BuildingUseAdjacent](../../psd/IfcProductExtension/Pset_BuildingUseAdjacent.xml){ target="SOURCE"}: specific property set for buildings to capture the use information about the adjacent buildings. 

****Quantity Use Definition****:

The quantities relating to the _IfcBuilding_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table border="1" cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1"><i><b>Name</b></i></font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1"><i><b>Description</b></i></font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i><b>Value Type</b></i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">NominalHeight</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated height of the
            building, measured from the level of terrain to the
            top part of the building. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityLength</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">NominalArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated coverage of the 
            site area that is occupied by the building (also
            referred to as footprint). The exact definition 
            and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossFloorArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated sum of all areas covered
            by the building</font> <font size="-1">(normally
            including the area of construction
            elements)</font><font size="-1">. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">NetFloorArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated sum of all usable areas
            covered by the building (normally excluding the area
            of construction elements). The exact definition and
            calculation rules depend on the method of measurement
            used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i> </font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossVolume</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated gross volume of all areas
            enclosed by the building</font> <font size="-1">(normally including the area of construction
            elements)</font><font size="-1">. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityVolume</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">NetVolume</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated net volume of all areas
            enclosed by the building</font> <font size="-1">(normally excluding the area of construction
            elements)</font><font size="-1">. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityVolume</i></font>
          </td>
        </tr>
      </tbody>
    </table>

****Spatial Structure Use Definition****

The _IfcBuilding_ is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship _IfcRelAggregates_. The _IfcBuilding_ references them by its inverse relationships:

*  _IfcBuilding.Decomposes_ -- referencing (_IfcSite_ || _IfcBuilding_) by _IfcRelAggregates.RelatingObject_, If it refers to another instance of _IfcBuilding_, the referenced _IfcBuilding_ needs to have a different and higher _CompositionType_, i.e. COMPLEX (if the other _IfcBuilding_ has ELEMENT), or ELEMENT (if the other _IfcBuilding_ has PARTIAL). 
*  _IfcBuilding.IsDecomposedBy_ -- referencing (_IfcBuilding_ || _IfcBuildingStorey_) by _IfcRelAggregates.RelatedObjects_. If it refers to another instance of _IfcBuilding_, the referenced _IfcBuilding_ needs to have a different and lower CompositionType, i.e. ELEMENT (if the other _IfcBuilding_ has COMPLEX), or PARTIAL (if the other _IfcBuilding_ has ELEMENT). 

If there are building elements and/or other elements
    directly related to the _IfcBuilding_ (like a curtain
    wall spanning several stories), they are associated with the
    _IfcBuilding_ by using the objectified relationship
    _IfcRelContainedInSpatialStructure_. The
    _IfcBuilding_ references them by its inverse
    relationship:  
*  _IfcBuilding.ContainsElements_ -- referencing any subtype of _IfcProduct_ (with the exception of other spatial structure element) by _IfcRelContainedInSpatialStructure.RelatedElements_. 

<table summary="Spatial structure">
      <tr>
        <td valign="top">
          <img src="figures/ifcbuilding-spatialstructure.png" alt="IfcBuilding as part of a spatial structure" width="501" height="451" border="0">
        </td>
        <td valign="top">
          <p>
            <small>Figure shows the <i>IfcBuilding</i> as
            part of the spatial structure. In this example, both
						the <i>IfcBuilding</i> and the referenced 
						<i>IfcBuildingStorey</i> have products contained.
						There is no definition on the level of product subtypes
						about which particular element can (only) be assigned
						to an <i>IfcBuilding</i> or an <i>IfcBuildingStorey</i></small>
          </p>
        </td>
      </tr>
    </table>

****Attribute Use Definition****:

<table border="1" cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <img src="figures/ifcbuilding-fig1.gif" alt="building heights" border="0" height="280" width="350"> 
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The heated space within a Building
              shall be handled by the <i>IfcZone</i>, including
              the property for overall height of the heated space
              in the Building. The following figure shall define
              the interpretation of building heights and
              elevations for <i>IfcBuilding</i>.</font>
            </p>
            <p>
              <font size="-1">The <i>ElevationOfRefHeight</i> is
              used to give the height above sea level of the
              internal height 0.00. The height 0.00 is often used
              as a building internal reference height and equal
              to the floor finish level of the ground
              floor.</font>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

****Geometry Use Definitions****:

The geometric representation of _IfcBuilding_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcBuilding_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if relative placement is used) to the _IfcSpatialStructureElement_ of type _IfcSite_, or of type _IfcBuilding_ (e.g. to position a building relative to a building complex, or a building section to a building). 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Currently, the use of a 2D 'FootPrint' representation of type 'GeometricCurveSet' and a 3D 'Body' representation of type 'Brep' is supported.

**Foot Print Representation**

The foot print representation of _IfcBuilding_ is given by either a single 2D curve (such as _IfcPolyline_ or _IfcCompositeCurve_), or by a list of 2D curves (in case of inner boundaries), if the building has an independent geometric representation.

The representation identifier and type of this geometric representation of _IfcBuilding_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint' 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' 

**Body Representation**

The body (or solid model) geometric representation (if the building has an independent geometric representation) of _IfcBuilding_ is defined using faceted B-Rep capabilities (with or without voids), based on the _IfcFacetedBrep_ or on the _IfcFacetedBrepWithVoids_.

The representation identifier and type of this representation of _IfcBuilding_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body' 
*  _IfcShapeRepresentation.RepresentationType_ = 'Brep' 

Since the building shape is usually described by the exterior building elements, an independent shape representation shall only be given, if the building is exposed independently from its constituting elements.