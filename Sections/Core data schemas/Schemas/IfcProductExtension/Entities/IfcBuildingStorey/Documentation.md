The building storey has an elevation and typically represents a (nearly) horizontal aggregation of spaces that are vertically bound.

A storey is (if specified) associated to a building. A storey may span over several connected storeys. Therefore storey complex provides for a collection of storeys included in a building. A storey can also be decomposed in (horizontal) parts, where each part defines a partial storey. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElements_ which is interpreted as follow:

* COMPLEX = building storey complex 
* ELEMENT = building storey 
* PARTIAL = partial building storey 

> <font size="-1">EXAMPLE: In split level houses, a storey is
      split into two or more partial storeys, each with a
      different elevation. It can be handled by defining a
      storey, which includes two or more partial storeys with the
      individual elevations.</font>

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
      Release 1.0</font>

****Property Set Use Definition****

The property sets relating to the _IfcBuildingStorey_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcBuildingStorey_ are part of this IFC release:

*  [Pset_BuildingStoreyCommon](../../psd/IfcProductExtension/Pset_BuildingStoreyCommon.xml){ target="SOURCE"}: common property set for all types of building stories 

****Quantity Use Definition****

The quantities relating to the building storey are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table border="1" cellpadding="2" cellspacing="2" summary="summary of base quantities available for IfcBuildingStorey">
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
            <font size="-1">Standard height of this storey, from
            the bottom surface of the floor, to the bottom
            surface of the floor or roof above. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityLength</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossFloorArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated sum of all areas covered
            by the building storey (as horizontal projections and
            normally including the area of construction elements.
            The exact definition and calculation rules depend on
            the method of measurement used.</font>
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
            covered by the building storey (normally excluding
            the area of construction elements). The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossVolume</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated gross volume of all areas
            enclosed by the building storey (</font><font size="-1">normally including the area of construction
            elements</font><font size="-1">). The exact
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
            enclosed by the building storey</font> <font size="-1">(normally excluding the area of construction
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

The _IfcBuildingStorey_ is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship _IfcRelAggregates_. The _IfcBuildingStorey_references them by its inverse relationships:

*  _IfcBuildingStorey.Decomposes_ -- referencing (_IfcBuilding_ || _IfcBuildingStorey_) by _IfcRelAggregates.RelatingObject_, If it refers to another instance of _IfcBuildingStorey_, the referenced _IfcBuildingStorey_ needs to have a different and higher _CompositionType_, i.e. COMPLEX (if the other _IfcBuildingStorey_ has ELEMENT), or ELEMENT (if the other _IfcBuildingStorey_ has PARTIAL). 
*  _IfcBuildingStorey.IsDecomposedBy_ -- referencing (_IfcBuildingStorey_ || _IfcSpace_) by _IfcRelAggregates.RelatedObjects_. If it refers to another instance of _IfcBuildingStorey_, the referenced _IfcBuildingStorey_ needs to have a different and lower CompositionType, i.e. ELEMENT (if the other _IfcBuildingStorey_ has COMPLEX), or PARTIAL (if the other _IfcBuildingStorey_ has ELEMENT). 

If there are building elements and/or other elements
    directly related to the _IfcBuildingStorey_ (like most
    building elements, such as walls, columns, etc.), they are
    associated with the _IfcBuildingStorey_ by using the
    objectified relationship
    _IfcRelContainedInSpatialStructure_. The
    _IfcBuildingStorey_ references them by its inverse
    relationship:  
*  _IfcBuildingStorey.ContainsElements_ -- referencing any subtype of _IfcProduct_ (with the exception of other spatial structure element) by _IfcRelContainedInSpatialStructure.RelatedElements_. 

<table summary="Spatial structure">
      <tr>
        <td valign="top">
          <img src="figures/ifcbuildingstorey-spatialstructure.png" alt="IfcBuildingStorey as part of a spatial structure" width="501" height="401" border="0">
        </td>
        <td valign="top">
          <p>
            <small>Figure shows the <i>IfcBuildingStorey</i> as
            part of the spatial structure. It also serves as the
						spatial container for building and other elements.</small>
          </p>
        </td>
      </tr>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcBuildingStorey_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcBuildingStorey_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if relative placement is used) to the _IfcSpatialStructureElement_ of type _IfcBuilding_, or of type _IfcBuildingStorey_ (e.g. to position a building storey relative to a building storey complex, or a partial building storey to a building storey). 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

****Geometric Representations****

Currently, the use of a 2D 'FootPrint' representation of type 'GeometricCurveSet' and a 3D 'Body' representation of type 'Brep' is supported.

> <small>NOTE The independent geometric representation of
        <i>IfcBuildingStorey</i> may not be required or allowed
        in certain view definitions. In those cases only the
        contained elements and spaces have an independent
        geometric representation.</small>
> 


**Foot Print Representation**

The foot print representation of _IfcBuildingStorey_ is given by either a single 2D curve (such as _IfcPolyline_ or _IfcCompositeCurve_), or by a list of 2D curves (in case of inner boundaries), if the building storey has an independent geometric representation.

The representation identifier and type of this geometric representation of _IfcBuildingStorey_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint' 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' 

**Body Representation**

The body (or solid model) geometric representation (if the building storey has an independent geometric representation) of _IfcBuildingStorey_ is defined using faceted B-Rep capabilities (with or without voids), based on the _IfcFacetedBrep_ or on the _IfcFacetedBrepWithVoids_.

The representation identifier and type of this representation of _IfcBuildingStorey_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body' 
*  _IfcShapeRepresentation.RepresentationType_ = 'Brep' 

Since the building storey shape is usually described by the exterior building elements, an independent shape representation shall only be given, if the building storey is exposed independently from its constituting elements.