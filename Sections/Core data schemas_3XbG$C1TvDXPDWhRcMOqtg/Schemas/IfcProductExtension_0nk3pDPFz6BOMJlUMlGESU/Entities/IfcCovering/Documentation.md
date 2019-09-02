**Definition from ISO 6707-1:1989**: term used: Finishing - final coverings and treatments of surfaces and their intersections.

A covering is an element which covers some part of another element and is fully dependent on that other element. The _IfcCovering_ defines the occurrence of a covering type, that (if given) is expressed by the _IfcCoveringType_.

> <small>EXAMPLEs include wall claddings, floorings and
        suspended ceilings as well as finish trim and base
        molding.</small>
> 


> <small><font color="#FF0000">IFC2x PLATFORM CHANGE: The
      attribute <i>PredefinedType</i> is now optional and should
      only be inserted when there is no type information, given
      by <i>IfcCoveringType</i>, is assigned to the
      <i>IfcCovering</i> occurrence by
      <i>IfcRelDefinesByType</i>.</font></small>

Coverings can be assigned to

* a space represented by _IfcSpace_ 
    * using the inverse relationship _CoversSpaces_ pointing to _IfcRelCoversSpaces_. The space is then accessible via _IfcRelCoversSpaces.RelatedSpace_.  
* a space boundary represented by _IfcRelSpaceBoundary_  
    * using the inverse relationship _ProvidesBoundaries_ pointing to _IfcRelSpaceBoundary._ The space is then accessible via _IfcRelSpaceBoundary.RelatingSpace_.  
* a building element represented by _IfcBuildingElement_ 
    * using the inverse relationship _Covers_ pointing to _IfcRelCoversBldgElements_. The building element is then accessible via _IfcRelCoversBldgElements.RelatingBuildingElement_.  
* a distribution element represented by _IfcDistributionElement_ 
    * using the inverse relationship _Covers_ pointing to _IfcRelCoversBldgElements_. The distribution element is then accessible via _IfcRelCoversBldgElements.RelatingBuildingElement_. Only _IfcCovering_'s with a PredefinedType INSULATION, MEMBRANE, SLEEVING, or WRAPPING shall be used to cover distribution elements.  

> <small><font color="#FF0000">IFC2x PLATFORM CHANGE With the
      upward compatible platform extension at
      <i>IfcRelCoversBldgElements</i> the <i>IfcCovering</i> can
      now also cover an <i>IfcElement</i> (and its subtypes in
      addition to <i>IfcBuildingElement</i>). Additional
      enumerators have been added to <i>IfcCoveringTypeEnum</i>
      to identify coverings applicable to elements other than
      building elements.</font></small>

The following guideline shall apply:

* (default) if the space has coverings that may not have an own shape representation and no defined relationships to the building elements they cover, then the _IfcCovering_ shall be assigned to _IfcSpace_ using the _IfcRelCoversSpaces_ relationship, 
* if the space has coverings that have an own shape representation and the space has defined space boundaries, then the covering, which relates to that space, may be assigned to the space boundaries using the link to _IfcRelSpaceBoundary,_ 
* if the covering does not relate to a space, then the covering should be assigned to the building element or a distribution element using the _IfcRelCoversBldgElements_ relationship. 

> <small><font color="#0000FF">HISTORY New entity in IFC
      Release 1.0.</font></small>

****Type Use Definition****

The _IfcCovering_ defines the occurrence of any covering, common information about covering types (or styles) is handled by _IfcCoveringType_. The _IfcCoveringType_ (if present) may establish the common type name, usage (or predefined) type, common set of properties, common material layer set, and common shape representations (using _IfcRepresentationMap_). The _IfcCoveringType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

As an additional use agreement for standard coverings (i.e. slabs with constant thickness along the extrusion direction), the _IfcCoveringType_ should have a unique _IfcMaterialLayerSet_, that is referenced by the _IfcMaterialLayerSetUsage_ assigned to all occurrences of this covering type.

<table border="0" cellpadding="2" cellspacing="2" width="100%">
      <tbody>
        <tr>
          <td>
            <p>
              <img alt="Material layer set and usage" src="figures/IfcCovering_MaterialUsage-01.png" height="220" width="501"> 
            </p>
          </td>
          <td align="left" valign="top">
            <p>
              <small>Assignment of
              <i>IfcMaterialLayerSetUsage</i> and
              <i>IfcMaterialLayerSet</i> to the covering type and the
              covering occurrence.</small>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

If an _IfcCoveringType_ is assigned to the _IfcCovering_, the attribute _PredefinedType_ shall not be assigned, or shall be identical to _IfcCoveringType.PredefinedType_.

****Property Set Use Definition****:

The property sets relating to the _IfcCovering_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcCovering_ are part of this IFC release:

*  [Pset_CoveringCommon](../../psd/IfcProductExtension/Pset_CoveringCommon.xml){ target="SOURCE"}: common property set for all covering occurrences 
    *  [Pset_CoveringCeiling](../../psd/IfcProductExtension/Pset_CoveringCeiling.xml){ target="SOURCE"}: specific property set for all occurrences of coverings with the PredefinedType: CEILING 
    *  [Pset_CoveringFlooring](../../psd/IfcProductExtension/Pset_CoveringFlooring.xml){ target="SOURCE"}: specific property set for all occurrences of coverings with the PredefinedType: FLOORING  

****Quantity Use Definition****:

The quantities relating to the _IfcCovering_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

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
        <tr>
          <td align="left" valign="top">
            <font size="-1">GrossArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Total area of the covering in the
            elevation view. The exact definition and calculation
            rules depend on the method of measurement
            used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
        <tr>
          <td align="left" valign="top">
            <font size="-1">NetArea</font>
          </td>
          <td align="left" valign="top">
            <font size="-1">Total area of the covering in the
            elevation view taking into account possible openings.
            The exact definition and calculation rules depend on
            the method of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
      </tbody>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcCovering_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation. Included are:

**Local Placement**

The local placement for _IfcCovering_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the same _IfcSpatialStructureElement_ , which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the _IfcCovering_, however, is assigned to an _IfcBuildingElement_, and this element defines its own local placement, than the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the _IfcBuildingElement_. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

_**Geometric Representations**_

The geometric representation of the _IfcCovering_ depends on two criteria:

1. Does it define an area or a volume? 
2. Is the base surface (either the _IfcRelSpaceBoundary_ or the surface of the _IfcBuildingElement_ it relates to) a planar surface or a cylindrical surface? 

**GeometricSet Representation**

The 'GeometricSet' geometric representation of _IfcCovering_ supports area definitions as 3D surfaces.

*  _RepresentationIdentifier_ : 'Surface' 
*  _RepresentationType_ : 'GeometricSet' 

The following additional constraints apply to the 'GeometricSet' representation of _IfcCovering_:

* for planar base surfaces - bounded surface representation 
* for cylindrical base surfaces - swept surface representation 

> EXAMPLE for standard geometric representation.

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcCovering_Standard-1-Layout1.dwf"><img src="figures/IfcCovering_Standard-1-Layout1.gif" alt="standard planar covering" border="0" height="274" width="399"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The area of <i>IfcCovering</i> is
              given by an <i>IfcPolyLoop</i> for planar base
              surfaces (here given by the
              <i>IfcRelSpaceBoundary</i>).</font>
            </p>
            <ul>
              <li>
                <font size="-1">The implicit planar surface of
                the <i>IfcPolyLoop</i> shall be identical with
                the planar surface defined by the
                <i>IfcRelSpaceBoundary</i>.</font>
              </li>
            </ul>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcCovering_Standard-2-Layout1.dwf"><img src="figures/IfcCovering_Standard-2-Layout1.gif" alt="standard cylindrical covering" border="0" height="274" width="399"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The area of the <i>IfcCovering</i>
              is given by an <i>IfcSurfaceOfLinearExtrusion</i>
              for cylindrical base surfaces (here given by the
              <i>IfcRelSpaceBoundary</i> - e.g. caused by a round
              wall).</font>
            </p>
            <ul>
              <li>
                <font size="-1">The geometry representation of
                the <i>IfcCovering</i> is given by the
                <font size="-1">IfcTrimmedCurve</font> (the
                Curve parameter of the
                <i>IfcArbitraryOpenProfileDef</i> - in cases of
                faceted representation also an
                <i>IfcPolyline</i>). It is extruded within the
                plane of the base surface using the <i>Depth</i>
                parameter of the
                <i>IfcSurfaceOfLinearExtrusion</i>.</font>
              </li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>

**SweptSolid Representation**

The 'SweptSolid' geometric representation of _IfcCovering_ supports volume definitions as 3D solids.

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SweptSolid' 

The following additional constraints apply to the 'SweptSolid' representation of _IfcCovering_:

* for planar base surfaces - swept area representation 
* for cylindrical base surfaces - swept area representation 

> EXAMPLE for advanced geometric representation.

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcCovering_Advanced-1-Layout1.dwf"><img src="figures/IfcCovering_Advanced-1-Layout1.gif" alt="advanded solid covering" border="0" height="274" width="399"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The volume of <i>IfcCovering</i> is
              given by an <i>IfcExtrudedAreaSolid</i> for planar
              base surfaces (here given by the
              <i>IfcRelSpaceBoundary</i>).</font>
            </p>
            <ul>
              <li>
                <font size="-1">The extruded area
                (<i>IfcArbitraryClosedProfileDef</i>) shall be
                coplanar to the surface defined by the
                <i>IfcRelSpaceBoundary</i>.</font>
              </li>
            </ul>
          </td>
        </tr>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcCovering_Advanced-2-Layout1.dwf"><img src="figures/IfcCovering_Advanced-2-Layout1.gif" alt="advanced solid covering" border="0" height="274" width="399"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The volume of the
              <i>IfcCovering</i> is given by an
              <i>IfcExtrudedAreaSolid</i> for cylindrical base
              surfaces (here given by the
              <i>IfcRelSpaceBoundary</i> - e.g. caused by a round
              wall).</font>
            </p>
            <ul>
              <li>
                <font size="-1">The geometry representation of
                the <i>IfcCovering</i> is given by the
                <i>IfcCompositeCurve</i> (the <i>OuterCurve</i>
                parameter of the
                <i>IfcArbitraryClosedProfileDef</i> - in cases of
                faceted representation also a closed
                <i>IfcPolyline</i>). It is extruded along the
                plane of the base surface using the <i>Depth</i>
                parameter of the
                <i>IfcSurfaceOfLinearExtrusion</i>.</font>
              </li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>