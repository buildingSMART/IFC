The opening element stands for opening, recess or chase, all reflecting voids. It represents a void within any element that has physical manifestation. Openings must be handled by all sectors and disciplines in AEC/FM industry, therefore the interoperability for opening elements is provided at this high level.

There are two different types of opening elements:

* an opening, where the thickness of the opening is greater or equal to the thickness of the element; 
* a recess or niche, where the thickness of the recess is smaller than the thickness of the element. 

The inherited attribute _ObjectType_ should be used to capture the differences,

* the attribute is set to '**Opening**' for an opening or 
* the attribute is set to '**Recess**' for a recess or niche. 
* If the value for _ObjectType_ is omitted, opening is assumed. 

An _IfcOpeningElement_ has to be inserted into a building element (all subtypes of _IfcBuildingElement_) by using the _IfcRelVoidsElement_ relationship. ~~It is also
      directly linked to the spatial structure of the project
      (and here normally to the _IfcBuildingStorey_) by
      using the _IfcRelContainedInSpatialStructure_
      relationship~~. <font color="#0000FF">It should not
      be linked directly to the spatial structure of the project,
      i.e. the inverse relationship <i>ContainedInStructure</i>
      shall be NIL. It is assigned to the spatial structure
      through the elements it penetrates</font>.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
      Release 1.0</font>

> <font color="#FF0000" size="-1">IFC2x PLATFORM CHANGE: The
      intermediate ABSTRACT supertypes <i>IfcFeatureElement</i>
      and <i>IfcFeatureSubtraction</i> have been added between
      <i>IfcElement</i> and <i>IfcOpeningElement</i> with upward
      compatibility.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcOpeningElement_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcOpeningElement_ are part of this IFC release:

*  [Pset_OpeningElementCommon](../../psd/IfcProductExtension/Pset_OpeningElementCommon.xml){ target="SOURCE"}: common property set for all opening occurrences 

****Quantity Use Definition****:

The quantities relating to the _IfcOpeningElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

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
            <font size="-1">Area of the opening as viewed by an
            elevation view (for wall openings) or as viewed by a
            ground floor view (for floor openings). The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
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
            <font size="-1">Volume of the opening. The exact
            definition and calculation rules depend on the method
            of measurement used.</font>
          </td>
          <td align="left" valign="top">
            <font size="-1"><i>IfcQuantityVolume</i></font>
          </td>
        </tr>
			</tbody>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcOpeningElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcOpeningElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ should point to the local placement of the same element, which is voided by the opening, i.e. referred to by _VoidsElement.RelatingBuildingElement_. 

**_Geometric Representation_**

Currently, the use of 'SweptSolid', 'Brep', and 'MappedRepresentation' representation is supported.

**Swept Solid Representation with Horizontal
      Extrusion**  
The 'SweptSolid' geometric representation of _IfcOpeningElement_, using horizontal extrusion direction (for walls), is defined using the swept area solid geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SweptSolid' 

The following additional constraints apply to the swept solid representation:

<ul>
      <li>
        <u>Solid</u>: <i>IfcExtrudedAreaSolid</i> is required,
        <font color="#0000FF">the set of
        <i>IfcShapeRepresentation.Items</i> may include a single,
        or multiple, instances of
        <i>IfcExtrudedAreaSolid</i>.</font>
      </li>
      <li>
        <u>Profile</u>: <i>IfcRectangleProfileDef</i>,
        <i>IfcCircleProfileDef</i> and
        <i>IfcArbitraryClosedProfileDef</i> shall be supported.
      </li>
      <li>
        <u>Extrusion</u>: The profile shall be extruded
        horizontally (i.e. perpendicular to the extrusion
        direction of the voided element), e.g. for wall openings,
        or vertically (i.e. in the extrusion direction of the
        voided element), e.g., for floor openings. <font color="#0000FF">If multiple instances of
        <i>IfcExtrudedAreaSolid</i> are used, the extrusion
        direction should be equal.</font>
      </li>
    </ul>
Special agreement for defining openings in round building elements, e.g., in round walls. The opening width, in case of a rectangular opening equal with the _IfcRectangleProfileDef.XDim_, is defined as the straight line distance between two parallel jambs. If the jambs are defined radial (to the center of the arc used to define the round wall) then the opening width is defined to be the outer arc length.

> <font size="-1">NOTE: In case of non-parallel jambs,
        <font color="#0000FF">the shape representation shall be a
        'SweptSolid' representation with vertical
        extrusion.</font></font>
> 


EXAMPLE for openings

<table cellpadding="2" cellspacing="2" width="80%">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top" width="400">
            <a href="drawings/IfcOpeningElement-Layout1.dwf"><img src="figures/ifcopeningelement-layout1.gif" alt="standard opening" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="top" width="530">
            <p>
              <small>The following interpretation of dimension
              parameter applies for rectangular openings:</small>
            </p>
            <ul>
              <li>
                <small><i>IfcRectangleProfileDef.YDim</i>
                interpreted as opening width</small>
              </li>
              <li>
                <small><i>IfcRectangleProfileDef.XDim</i>
                interpreted as opening height</small>
              </li>
            </ul>
            <p>
              <small>NOTE: Rectangles are now defined centric,
              the placement location has to be set:</small>
            </p>
            <ul>
              <li>
                <i><small>IfcCartesianPoint(XDim/2,YDim/2)</small></i>
              </li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>

EXAMPLE for recesses

<table cellpadding="2" cellspacing="2" width="80%">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcOpeningElement-Recess-Layout1.dwf"><img src="figures/ifcopeningelement-recess-layout1.png" alt="recess" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <small>The following interpretation of dimension
              parameter applies for rectangular recess:</small>
            </p>
            <ul>
              <li>
                <small><i>IfcRectangleProfileDef.YDim</i>
                interpreted as recess width</small>
              </li>
              <li>
                <small><i>IfcRectangleProfileDef.XDim</i>
                interpreted as recess height</small>
              </li>
              <li>
                <small><i>IfcExtrudedAreaSolid.Depth</i> is
                interpreted as recess depth</small>
              </li>
            </ul>
            <p>
              <small>NOTE: Rectangles are now defined centric,
              the placement location has to be set:</small>
            </p>
            <ul>
              <li>
                <small><i>IfcCartesianPoint</i>(XDim/2,YDim/2)</small>
              </li>
            </ul>
            <p>
              <small>NOTE: The local placement directions for the
              <i>IfcOpeningElement</i> are only given as an
              example, other directions are valid as
              well.</small>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

> <small>NOTE  In case of recesses also profiles of type
        <i>IfcArbitraryProfileDefWithVoid</i> shall be supported
        as a 'SweptSolid' representation.</small>
> 


**Swept Solid Representation with Vertical
      Extrusion**  
The 'SweptSolid' geometric representation of _IfcOpeningElement_, using vertical extrusion direction (for walls), is defined using the swept area solid geometry, however the extrusion direction may be vertical, i.e. in case of a wall opening, the extrusion would be in the direction of the wall height. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SweptSolid' 

The following additional constraints apply to the swept solid representation:

<ul>
      <li>
        <u>Solid</u>: <i>IfcExtrudedAreaSolid</i> is required,
        <font color="#0000FF">the set of
        <i>IfcShapeRepresentation.Items</i> may include a single,
        or multiple, instances of
        <i>IfcExtrudedAreaSolid</i>.</font>
      </li>
      <li>
        <u>Profile</u>: <i>IfcRectangleProfileDef</i>,
        <i>IfcCircleProfileDef</i> and
        <i>IfcArbitraryClosedProfileDef</i> shall be supported.
      </li>
      <li>
        <u>Extrusion</u>: The profile shall be extruded
        vertically, i.e. for wall openings along the extrusion
        direction of the voided element.  <font color="#0000FF">If multiple instances of
        <i>IfcExtrudedAreaSolid</i> are used, the extrusion
        direction should be equal.</font>
      </li>
    </ul>
Vertical extrusions shall be used when an opening or
    recess has a non rectangular foot print geometry that does
    not change along the height of the opening or recess.  
**Brep Representation**  
The general b-rep geometric representation of _IfcOpeningElement_ is defined using the Brep geometry. The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'Brep'