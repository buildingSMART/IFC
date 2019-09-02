A space represents an area or volume bounded actually or theoretically. Spaces are areas or volumes that provide for certain functions within a building.

A space is (if specified) associated to a building storey (or in case of exterior spaces to a site). A space may span over several connected spaces. Therefore a space group provides for a collection of spaces included in a storey. A space can also be decomposed in parts, where each part defines a partial space. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElement_ which is interpreted as follow:

* COMPLEX = space group 
* ELEMENT = space 
* PARTIAL = partial space 

The following guidelines should apply for using the _Name_, _Description_, _LongName_ and _ObjectType_ attributes.

*  _Name_ holds the unique name (or space number) from the plan. 
*  _Description_ holds any additional information field the user may have specified, there are no further recommendations. 
*  _LongName_ holds the full name of the space, it is often used in addition to the _Name_, if a number is assigned to the room, then the descriptive name is exchanged as _LongName_. 
*  _ObjectType_ holds the space type, i.e. usually the functional category of the space . 

> <small><font color="#0000FF">HISTORY New Entity in IFC
        Release 1.0</font></small>
> 


****Property Set Use Definition****:

The property sets relating to the _IfcSpace_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcSpace_ are part of this IFC release:

*  [Pset_SpaceCommon](../../psd/IfcProductExtension/Pset_SpaceCommon.xml){ target="SOURCE"}: common property set for all types of spaces 
    *  [Pset_SpaceParking](../../psd/IfcProductExtension/Pset_SpaceParking.xml){ target="SOURCE"}: specific property set for only those spaces that are used to define parking spaces by _ObjectType_ = 'Parking' 
    *  [Pset_SpaceParkingAisle](../../psd/IfcProductExtension/Pset_SpaceParkingAisle.xml){ target="SOURCE"}: specific property set for only those spaces that are used to define parking aisle by _ObjectType_ = 'ParkingAisle'  
*  [Pset_SpaceFireSafetyRequirements](../../psd/IfcProductExtension/Pset_SpaceFireSafetyRequirements.xml){ target="SOURCE"}: common property set for all types of spaces to capture the fire safety requirements 
*  [Pset_SpaceLightingRequirements](../../psd/IfcProductExtension/Pset_SpaceLightingRequirements.xml){ target="SOURCE"}: common property set for all types of spaces to capture the lighting requirements 
*  [Pset_SpaceOccupancyRequirements](../../psd/IfcProductExtension/Pset_SpaceOccupancyRequirements.xml){ target="SOURCE"}: common property set for all types of spaces to capture the occupancy requirements 
*  [Pset_SpaceThermalRequirements](../../psd/IfcProductExtension/Pset_SpaceThermalRequirements.xml){ target="SOURCE"}: common property set for all types of spaces to capture the thermal requirements 
*  [Pset_SpaceThermalDesign](../../psd/IfcSharedBldgServiceElements/Pset_SpaceThermalDesign.xml){ target="SOURCE"}: common property set for all all types of spaces to capture building service design values 

****Quantity Use Definition****:

The quantities relating to the _IfcSpace_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table border="1" cellpadding="2" cellspacing="2" summary="quantity use definition">
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
            <font size="-1">Floor Height (without flooring) to
            Ceiling height (without suspended ceiling) for this
            space (measured from top of slab of this space to the
            bottom of slab of space above); the average shall be
            taken if room shape is not prismatic.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1">IfcQuantityLength</font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">ClearHeight</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Clear Height between floor level
            (including finish) and ceiling level (including
            finish and sub construction) of this space; the
            average shall be taken if room shape is not
            prismatic.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1">IfcQuantityLength</font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossPerimeter</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated gross</font> <font size="-1">perimeter at the floor level of this space.
            It </font><font size="-1">all sides of the space,
            including those parts of the perimeter that are
            created by virtual boundaries and openings. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1">IfcQuantityLength</font>
          </td>
        </tr>
        <tr>
          <td>
            <font size="-1">NetPerimeter</font>
          </td>
          <td>
            <font size="-1">Calculated net p</font><font size="-1">erimeter at the floor level of this space.
            It </font><font size="-1">normally</font> <font size="-1">excludes those parts of the perimeter that are
            created by</font> <font size="-1">by virtual
            boundaries and openings.</font> <font size="-1">The
            exact definition and calculation rules depend on the
            method of measurement used.</font>
          </td>
          <td>
            <font size="-1">IfcQuantityLength</font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <font size="-1">GrossFloorArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Calculated sum of all floor areas
            covered by the space. It</font> <font size="-1">normally includes the area covered
            by elements</font><font size="-1">inside the space
            (columns, inner walls, etc.). The exact definition
            and calculation rules depend on the method of
            measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr valign="top">
          <td>
            <font size="-1">NetFloorArea</font>
          </td>
          <td>
            <font size="-1">Calculated sum of all usable floor
            areas covered by the space. It normally excludes the
            area </font><font size="-1">covered</font>
            <font size="-1">by elements</font> <font size="-1">inside the space (columns, inner walls,
            etc.)</font><font size="-1">, floor openings, or
            other protruding elements. Special rules apply for
            areas that have a low headroom. The exact definition
            and calculation rules depend on the method of
            measurement used.</font>
          </td>
          <td>
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr>
          <td valign="top">
            <font size="-1">GrossCeilingArea</font>
          </td>
          <td valign="top">
            <font size="-1">Calculated sum of all ceiling areas
            of the space. It</font> <font size="-1">normally
            includes the area covered
            by elements</font><font size="-1">inside the space
            (columns, inner walls, etc.). The ceiling area is the
            real (and not the projected) area (e.g. in case of
            sloped ceilings). The exact definition and
            calculation rules depend on the method of measurement
            used.</font>
          </td>
          <td valign="top">
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr>
          <td valign="top">
            <font size="-1">NetCeilingArea</font>
          </td>
          <td valign="top">
            <font size="-1">Calculated sum of all ceiling areas
            covered by the space. It normally excludes the
            area</font> <font size="-1">covered
            by elements</font> <font size="-1">inside the space
            (columns, inner walls, etc.) or by ceiling
            openings</font><font size="-1">.</font> <font size="-1">The ceiling area is the real (and not the
            projected) area (e.g. in case of sloped
            ceilings).</font> <font size="-1">The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td valign="top">
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr>
          <td valign="top">
            <font size="-1">GrossWallArea</font>
          </td>
          <td valign="top">
            <font size="-1">Calculated sum of all wall areas
            bounded by the space. It</font> <font size="-1">normally includes the area </font><font size="-1">covered</font> <font size="-1">by elements</font><font size="-1">inside the
            wall area (doors, windows, other openings, etc.). The
            exact definition and calculation rules depend on the
            method of measurement used.</font>
          </td>
          <td valign="top">
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr>
          <td valign="top">
            <font size="-1">NetWallArea</font>
          </td>
          <td valign="top">
            <font size="-1">Calculated sum of all wall
            areas </font><font size="-1">bounded by</font>
            <font size="-1">the space. It normally
            excludes</font> <font size="-1">the area
            covered</font><font size="-1">by elements</font>
            <font size="-1">inside the wall area
            (</font><font size="-1">doors, windows, other
            openings, etc</font><font size="-1">.)</font><font size="-1">. Special rules apply
            for areas that have a low headroom. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td valign="top">
            <font size="-1">IfcQuantityArea</font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left">
            <font size="-1">GrossVolume</font>
          </td>
          <td align="left" width="60%">
            <font size="-1">Calculated gross volume of all areas
            enclosed by the space</font> <font size="-1">(normally including the volume of construction
            elements</font> <font size="-1">inside the
            space</font><font size="-1">)</font><font size="-1">.
            The exact definition and calculation rules depend on
            the method of measurement used.</font>
          </td>
          <td align="left">
            <font size="-1">IfcQuantityVolume</font>
          </td>
        </tr>
        <tr valign="top">
          <td align="left">
            <font size="-1">NetVolume</font>
          </td>
          <td align="left">
            <font size="-1">Calculated net volume of all areas
            enclosed by the space (normally excluding the volume
            of construction elements</font> <font size="-1">inside the space</font><font size="-1">). The
            exact definition and calculation rules depend on the
            method of measurement used.</font>
          </td>
          <td align="left">
            <font size="-1">IfcQuantityVolume</font>
          </td>
        </tr>
      </tbody>
    </table>

****Spatial Structure Use Definition****

The _IfcSpace_ is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship _IfcRelAggregates_. The _IfcSpace_ references them by its inverse relationships:

*  _IfcSpace.Decomposes_ -- referencing (_IfcSite_ || _IfcBuildingStorey_ || _IfcSpace_) by _IfcRelAggregates.RelatingObject_, If it refers to another instance of _IfcSpace_, the referenced _IfcSpace_ needs to have a different and higher _CompositionType_, i.e. COMPLEX (if the other _IfcSpace_ has ELEMENT), or ELEMENT (if the other _IfcSpace_ has PARTIAL). 
*  _IfcSpace.IsDecomposedBy_ -- referencing (_IfcSpace_) by _IfcRelAggregates.RelatedObjects_. If it refers to another instance of _IfcSpace_, the referenced _IfcSpace_ needs to have a different and lower _CompositionType_, i.e. ELEMENT (if the other _IfcSpace_ has COMPLEX), or PARTIAL (if the other _IfcSpace_ has ELEMENT). 

If there are building elements and/or other elements
    directly related to the _IfcSpace_ (like most furniture
    and distribution elements), they are associated with the
    _IfcSpace_ by using the objectified relationship
    _IfcRelContainedInSpatialStructure_. The _IfcSpace_
    references them by its inverse relationship:  
*  _IfcSpace.ContainsElements_ -- referencing any subtype of _IfcProduct_ (with the exception of other spatial structure element) by _IfcRelContainedInSpatialStructure.RelatedElements_. 

****Attribute Use Definition****:
    <table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td>
            <img src="figures/IfcSpace_Fig1.gif" alt="space heights" border="0" height="308" width="313">
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The following figure describes the
              heights and elevations of the
              <i>IfcSpace</i>.</font>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcSpace_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

> <font size="-1">NOTE1 If the surrounding instances of
        <i>IfcRelSpaceBoundary</i> define a complete geometric
        representation of a particular representation view for
        that space, then this view shall be omitted from the
        multiple representations of <i>IfcSpace</i>.</font>
> 


> <font size="-1">NOTE2 In cases of inconsistency between
        the geometric representation of the <i>IfcSpace</i> and
        its surrounding <i>IfcRelSpaceBoundary</i>, the geometric
        representation of the space should take priority over the
        geometric representation of the surrounding space
        boundaries</font>.
> 


**Local Placement**

The local placement for _IfcSpace_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the _IfcSpatialStructureElement_ of type "IfcBuildingStorey", if relative placement is used, or of type "IfcSpace" (e.g. to position a space relative to a space group, or a partial space to a space). 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Currently, the use of a 2D 'FootPrint' representation of type 'Curve2D' or 'GeometricCurveSet' and a 3D 'Body' representation of type 'SweptSolid, 'Clipping' and 'Brep' is supported.

**'Foot' Print representation**

The 2D geometric representation of _IfcSpace_ is defined using the 'Curve2D' or 'GeometricCurveSet' geometry. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'Curve2D' or 'GeometricCurveSet' . 

The following constraints apply to the 2D representation:

*  **Profile**: _IfcBoundedCurve_ is required, using _IfcPolyline_ for faceted space contours or _IfcCompositeCurve_ for space contours with arc segments. For spaces with inner boundaries, a set of _IfcBoundedCurve_'s is used, that should be grouped into an _IfcGeometricCurveSet_. 

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcSpace_2D-Layout1.dwf"><img src="figures/IfcSpace_2D-Layout1.gif" alt="2d representation" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">Two-dimensional bounded curve
              representing the foot print of
              <i>IfcSpace</i>.</font>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

**'Swept Solid' representation**

The standard geometric representation of _IfcSpace_ is defined using the swept area solid geometry. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'SweptSolid'. 

The following constraints apply to the standard representation:

*  **Solid**: _IfcExtrudedAreaSolid_ is required, 
*  **Profile**: _IfcArbitraryClosedProfileDef_ is required, _IfcArbitraryProfileDefWithVoids_ shall be supported. 
*  **Extrusion**: The extrusion direction shall be vertically, i.e., along the positive Z Axis of the co-ordinate system of the containing spatial structure element. 

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcSpace_Standard-Layout1.dwf"><img src="figures/IfcSpace_Standard-Layout1.gif" alt="fig1" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">Extrusion of an arbitrary profile
              definition with voids into the swept area solid of
              <i>IfcSpace</i>.</font>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

**'Clipping' representation**

The advanced geometric representation of _IfcSpace_ is defined using the swept area solid geometry that can be subjected to a Boolean expression. The following attribute values should be inserted.

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'Clipping'. 

The following additional constraints apply to the advanced representation:

*  **Solid**: see standard geometric representation, 
*  **Profile**: see standard geometric representation, 
*  **Extrusion**: see standard geometric representation, 
*  **Boolean result**: The difference operation with the second operand being of type _IfcHalfSpaceSolid_ (or one of its subtypes) shall be supported. 

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcSpace_Advanced-Layout1.dwf"><img src="figures/IfcSpace_Advanced-Layout1.gif" alt="fig2" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="top">
            <font size="-1">Extrusion of an arbitrary profile
            definition into the swept area solid. The solid and
            an half space solid are operands of the Boolean
            result of <i>IfcSpace</i>.</font>
          </td>
        </tr>
      </tbody>
    </table>

**'Brep' representation**

The fallback advanced geometric representation of _IfcSpace_ is defined using the Brep solid geometry. may be represented as a single or multiple instances of _IfcFacetedBrep_ or _IfcFacetedBrepWithVoids_. The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _IfcShapeRepresentation.__RepresentationIdentifier_ : 'Body' 
*  _IfcShapeRepresentation.__RepresentationType_ : 'Brep'