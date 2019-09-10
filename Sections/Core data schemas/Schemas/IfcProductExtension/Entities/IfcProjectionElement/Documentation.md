The _IfcProjectionElement_ is a specialization of the general feature element to represent projections applied to building elements. It represents a solid attached to any element that has physical manifestation. Projections must be handled by all sectors and disciplines in AEC/FM industry, therefore the interoperability for opening elements is provided at this high level.

> <font size="-1">EXAMPLE: A wall projection such as a
      pilaster strip is handled by
      <i>IfcProjectionElement</i></font>

An _IfcProjectionElement_ has to be linked to a building element (all subtypes of _IfcBuildingElement_) by using the _IfcRelProjectsElement_ relationship. Its existence depends on the existence of the master element.  
~~It is also directly linked to the spatial structure
      of the project (and here normally to the
      _IfcBuildingStorey_) by using the
      _IfcRelContainedInSpatialStructure_
      relationship~~. <font color="#0000FF">It should not
      be linked directly to the spatial structure of the project,
      i.e. the inverse relationship <i>ContainedInStructure</i>
      shall be NIL. It is assigned to the spatial structure
      through the element it projects.</font>

> <font color="#0000FF" size="-1">HISTORY New entity in
      Release IFC2x Edition 2.</font>

****Quantity Use Definition****:

The quantities relating to the _IfcProjectionElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

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
            <font size="-1">NominalArea</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Area of the projection as viewed by
            an elevation view (for wall projection) or as viewed
            by a ground floor view (for slab projection). The
            exact definition and calculation rules depend on the
            method of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityArea</i></font>
          </td>
        </tr>
        <tr>
          <td align="left" valign="top">
            <font size="-1">NominalVolume</font>
          </td>
          <td align="left" valign="top" width="60%">
            <font size="-1">Volume of the projection. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityVolume</i></font>
          </td>
        </tr>
      </tbody>
    </table>

****Geometry Use Definition****

The geometric representation of _IfcProjectionElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcOpeningRecess_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ should point to the local placement of the same element, to which the projection adds, i.e. referred to by _ProjectsElement.RelatingBuildingElement_. 

**Swept Solid Representation**

The geometric representation of _IfcProjectionElement_ is defined using the swept area solid geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SweptSolid' 

The following additional constraints apply to the swept solid representation:

*  **Solid**: _IfcExtrudedAreaSolid_ is required. 
*  **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_ and _IfcArbitraryClosedProfileDef_ shall be supported. 
*  **Extrusion**: The profile shall be extruded horizontally (i.e. perpendicular to the extrusion direction of the modified element), e.g. for wall projections, or vertically (i.e. in the extrusion direction of the projected element), e.g., for floor projections. 

EXAMPLE

<table cellpadding="2" cellspacing="2">
      <tr valign="top">
        <td valign="top" align="left">
          <a href="drawings/IfcProjectionElement-Layout1.dwf"><img src="figures/ifcprojectionelement-layout1.png" alt="projection" width="400" height="300" border="0"></a>
        </td>
        <td valign="top" align="left">
          <p>
            The following interpretation of dimension parameter
            applies for rectangular projection:
          </p>
          <ul>
            <li>
              <i>IfcRectangleProfileDef.YDim</i> interpreted as
              projection width
            </li>
            <li>
              <i>IfcRectangleProfileDef.XDim</i> interpreted as
              projection height
            </li>
            <li>
              <i>IfcExtrudedAreaSolid.Depth</i> is interpreted as
              projection depth
            </li>
          </ul>
          <p>
            NOTE: Rectangles are now defined centric, the
            placement location has to be set:
          </p>
          <ul>
            <li>
              <i>IfcCartesianPoint</i>(XDim/2,YDim/2)
            </li>
          </ul>
          <p>
            NOTE: The local placement directions for the
            <i>IfcProjectionElement</i> are only given as an
            example, other directions are valid as well.
          </p>
        </td>
      </tr>
    </table>

**Brep Representation**

The general b-rep geometric representation of _IfcProjectionElement_ is defined using the Brep geometry. The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'Brep'