**Definition from ISO 6707-1:1989**: Area where construction works are undertaken.

A defined area of land, possibly covered with water, on which the project construction is to be completed. A site may be used to erect building(s) or other AEC products.

A site (_IfcSite_) may include a definition of the single geographic reference point for this site (global position using _Longitude_, _Latitude_ and _Elevation_) for the project. This definition may specify an exact global position of the origin of the local placement of the IfcSite in geospatial terms or it may specify an approximate position intended for informational purposes only.

The geometrical placement of the site, defined by the _IfcLocalPlacement_, shall be always relative to the spatial structure element, in which this site is included, or absolute, i.e. to the world coordinate system, as established by the geometric representation context of the project. The world coordinate system, established at the _IfcProject.RepresentationContexts_, may include a definition of the true north within the XY plane of the world coordinate system, if provided, it can be obtained at _IfcGeometricRepresentationContext.TrueNorth_.

A project may span over several connected or disconnected sites. Therefore site complex provides for a collection of sites included in a project. A site can also be decomposed in parts, where each part defines a site section. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElements_ which is interpreted as follow:

* COMPLEX = site complex 
* ELEMENT = site 
* PARTIAL = site section 

> <small><font color="#0033FF">HISTORY  New entity in IFC
      Release 1.0.</font></small>

****Property Set Use Definition****

The property sets relating to the _IfcSite_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcSite_ are part of this IFC release:

*  [Pset_SiteCommon](../../psd/IfcProductExtension/Pset_SiteCommon.xml){ target="SOURCE"}: common property set for all types of site 

****Quantity Use Definition****

The quantities relating to the _IfcSite_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelAssignsProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" summary="quantity use definition">
      <tbody>
        <tr>
          <td>
            <font size="-1"><i><b>Name</b></i></font>
          </td>
          <td>
            <font size="-1"><i><b>Description</b></i></font>
          </td>
          <td>
            <font size="-1"><i><b>Value Type</b></i></font>
          </td>
        </tr>
        <tr>
          <td>
            <font size="-1">NominalPerimeter</font>
          </td>
          <td>
            <font size="-1">Perimeter of the Site boundary. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td>
            <font size="-1"><i>IfcQuantityLength</i></font>
          </td>
        </tr>
        <tr>
          <td>
            <font size="-1">NominalArea</font>
          </td>
          <td>
            <font size="-1">Area for this site (horizontal
            projections). The exact definition and calculation 
						rules depend on the method of measurement used.</font>
          </td>
          <td>
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
      </tbody>
    </table>

****Spatial Structure Use Definition****

The _IfcSite_ is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship _IfcRelAggregates_. The _IfcSite_ references them by its inverse relationships:

*  _IfcSite.Decomposes_ -- referencing (_IfcProject_ || _IfcSite_) by _IfcRelAggregates.RelatingObject_, If it refers to another instance of _IfcSite_, the referenced _IfcSite_ needs to have a different and higher _CompositionType_, i.e. COMPLEX (if the other _IfcSite_ has ELEMENT), or ELEMENT (if the other _IfcSite_ has PARTIAL). 
*  _IfcSite.IsDecomposedBy_ -- referencing (_IfcSite_ || _IfcBuilding_ || _IfcSpace_) by _IfcRelAggregates.RelatedObjects_. If it refers to another instance of _IfcSite_, the referenced _IfcSite_ needs to have a different and lower CompositionType, i.e. ELEMENT (if the other _IfcSite_ has COMPLEX), or PARTIAL (if the other _IfcSite_ has ELEMENT). 

If there are building elements and/or other elements
    directly related to the _IfcSite_ (like a fence, or a
    shear wall), they are associated with the _IfcSite_ by
    using the objectified relationship
    _IfcRelContainedInSpatialStructure_. The
    _IfcIfcSite_ references them by its inverse
    relationship:  
*  _IfcSite.ContainsElements_ -- referencing any subtype of _IfcProduct_ (with the exception of other spatial structure element) by _IfcRelContainedInSpatialStructure.RelatedElements_. 

<table summary="Spatial and placement structure">
      <tr>
        <td valign="top">
          <img src="figures/ifcsite-spatialstructure.png" alt="IfcSite as part of a spatial structure" width="501" height="461" border="0">
        </td>
        <td valign="top">
          <p>
            <small>Figure shows the <i>IfcSite</i> as
            part of the spatial structure. In addition to the 
						logical spatial structure, also the placement
						hierarchy is shown. In this example the spatial
						structure hierarchy and the placement hierarchy are
						identical.</small>
          </p>
					<p><small>NOTE  View definitions and implementation
					guidelines may require both hierarchies to be
					identical.</small>
					</p>
        </td>
      </tr>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcSite_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local placement**

The local placement for _IfcSite_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the _IfcSpatialStructureElement_ of type "_IfcSite_", if relative placement is used (e.g. to position a site relative a a site complex, or a site section to a site). 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. If there is only one site object, then this is the default situation. 

**Foot Print Representation**

The foot print representation of _IfcSite_ is given by either a single 2D curve (such as _IfcPolyline_ or _IfcCompositeCurve_), or by a list of 2D curves (in case of inner boundaries).

The representation identifier and type of this geometric representation of _IfcSite_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint' 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' 

**Survey Points Representation**

The survey point representation of _IfcSite_ is defined using a set of survey points and optionally breaklines. The breaklines are restricted to only connect points given in the set of survey points. Breaklines, if given, are used to constrain the triangulation.

The representation identifier and type of this geometric representation of _IfcSite_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'SurveyPoints' 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricSet' 

<table cellpadding="2" cellspacing="2" summary="survey points representation">
      <tbody>
        <tr>
          <td>
            <img src="figures/ifcsite-standard-points.gif" alt="points only" border="0" height="300" width="400">
          </td>
          <td align="left" valign="top">
            <p>
              A set of survey points, given as 3D Cartesian
              points within the object coordinate system of the
              site.
            </p>
            <p>
              The set of <i>IfcCartesianPoint</i> is included in
              the set of <i>IfcGeometricSet.Elements</i>.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <img src="figures/ifcsite-standard-facets-points.gif" alt="facetation of points" border="0" height="300" width="400">
          </td>
          <td align="left" valign="top">
            result after facetation
          </td>
        </tr>
        <tr>
          <td>
            <img src="figures/ifcsite-standard-breaklines.gif" alt="breaklines" border="0" height="300" width="400">
          </td>
          <td align="left" valign="top">
            <p>
              A set of survey points, given as 3D Cartesian
              points, and a set of break points, given as a set
              of lines, connecting some survey points, within the
              object coordinate system of the site.
            </p>
            <p>
              The set of <i>IfcCartesianPoint</i> and the set of
              <i>IfcPolyline</i> are included in the set of
              <i>IfcGeometricSet.Elements</i>.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <img src="figures/ifcsite-standard-facets-breaklines.gif" alt="facetation with breakpoints" border="0" height="300" width="400">
          </td>
          <td align="left" valign="top">
            result after facetation taking the breaklines into
            account.
          </td>
        </tr>
      </tbody>
    </table>

> <small>NOTE  The geometric representation of the site has
      been based on the ARM level description of the
      site_shape_representation given within the ISO 10303-225
      "Building Elements using explicit shape
      representation".</small>

**Facetation Representation**

The facetation representation of _IfcSite_ is defined using a surface model, based on the _IfcFaceBasedSurfaceModel_ or on the _IfcShellBasedSurfaceModel_. Normally the surface model is the result after triangulation of the site survey points.

The representation identifier and type of this representation of _IfcSite_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Facetation' 
*  _IfcShapeRepresentation.RepresentationType_ = 'SurfaceModel' 

**Body Representation**

The body (or solid model) representation of _IfcSite_ is defined using a faceted boundary representation based on the _IfcFacetedBrep_ or on the _IfcFacetedBrepWithVoids_.

The representation identifier and type of this representation of _IfcSite_ is:

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Body' 
*  _IfcShapeRepresentation.RepresentationType_ = 'Brep'
