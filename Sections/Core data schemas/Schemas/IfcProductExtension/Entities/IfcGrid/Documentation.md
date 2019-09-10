_IfcGrid_ ia a planar design grid defined in 3D space used as an aid in locating structural and design elements. The position of the grid (_ObjectPlacement_) is defined by a 3D coordinate system (and thereby the design grid can be used in plan, section or in any position relative to the world coordinate system). The position can be relative to the object placement of other products or grids. The XY plane of the 3D coordinate system is used to place the grid axes, which are 2D curves (e.g., line, circle, trimmed curve, polyline, or composite curve).

The inherited attributes _Name_ and _Description_ can be used to define a descriptive name of the grid and to indicate the grid's purpose. A grid is defined by (normally) two, or (in case of a triangular grid) three lists of grid axes. The following table shows some examples.

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td width="320">
            <img src="figures/ifcdesigngrid-type1.gif" alt="1" border="0" height="211" width="306">
          </td>
          <td align="left" valign="top" width="320">
            <img src="figures/ifcdesigngrid-type2.gif" alt="2" border="0" height="211" width="306">
          </td>
          <td width="320">
            <img src="figures/ifcdesigngrid-type3.gif" alt="3" border="0" height="211" width="306">
          </td>
        </tr>
        <tr>
          <td width="320">
            rectangular grid
          </td>
          <td align="left" valign="top" width="320">
            radial grid
          </td>
          <td valign="top" width="320">
            triangular grid
          </td>
        </tr>
      </tbody>
    </table>

The grid axes, defined within the design grid, are those elements to which project objects will be placed relatively using the _IfcGridPlacement_.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
      Release 1.0.</font>

**Informal Proposition**

1. Grid axes, which are referenced in different lists of axes (UAxes, VAxes, WAxes) shall not be parallel. 
2. Grid axes should be defined such as there are no two grid axes which intersect twice. 

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top" width="320">
            <img src="figures/ifcdesigngrid-ip2.gif" alt="IP2" border="0" height="97" width="306">
          </td>
          <td align="left" valign="top">
            Informal Proposition #2
            <ul>
              <li>left side: ambiguous intersections A1 and A2, a
              grid containing such grid axes is not a valid
              design grid.
              </li>
              <li>right side: the conflict can be resolved by
              splitting one grid axis in a way, such as no
              ambiguous intersections exist.
              </li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>

****Geometry Use Definitions****

The geometric representation of _IfcGrid_ is given by the _IfcProductDefinitionShape_, allowing geometric representations. Included are:

**Local Placement**

The local placement for _IfcGrid_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Currently, the use of a 2D 'FootPrint' representation of type 'GeometricCurveSet' is supported.

**GeometricCurveSet representation**

The 2D geometric representation of _IfcGrid_ is defined using the 'GeometricCurveSet' geometry. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' . 

The following constraints apply to the 2D representation:

* The _IfcGeometricCurveSet_ shall be an (and the only) _Item_ of the _IfcShapeRepresentation_. It should contain an _IfcGeometricCurveSet_ containing subtypes of _IfcCurve_, each representing a grid axis. Applicable subtypes of _IfcCurve_ are: _IfcPolyline_, _IfcCircle_, _IfcTrimmedCurve_ (based on _BaseCurve_ referencing _IfcLine_ or _IfcCircle_).  
* Each subtype of _IfcCurve_ may have a curve style assigned, using _IfcAnnotationCurveOccurrence_ referencing _IfcCurveStyle_. 
* Optionally the grid axis labels may be added as _IfcTextLiteral_, and they may have text styles assigned, using _IfcAnnotationTextOccurrence_ referencing _IfcTextStyle_. 

_Illustrations_

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td>
            <a href="drawings/IfcDesignGrid-Layout1.dwf"><img src="figures/ifcdesigngrid-layout1.gif" alt="design grid" border="0" height="300" width="400"></a>
          </td>
          <td align="left" valign="bottom">
            <p>
              <small>The <i>IfcGrid</i> defines a placement
              coordinate system using the <i>ObjectPlacement</i>.
              The XY plane of the coordinate system is used to
              place the 2D grid axes. The <i>Representation</i>
              of <i>IfcGrid</i> is defined using
              <i>IfcProductRepresentation</i>, referencing an
              <i>IfcShapeRepresentation</i>, that
              includes <i>IfcGeometricCurveSet</i> as
              <i>Items</i>. All grid axes are added as
              <i>IfcPolyline</i> to the
              <i>IfcGeometricCurveSet</i>.</small>
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <img src="figures/ifcgrid-representation.png" alt="representation of a design grid" width="501" height="621" border="0">
          </td>
          <td align="left" valign="bottom">
            <p>
              <small>The attributes <i>UAxes</i> and <i>VAxes</i>
              define lists of <i>IfcGridAxis</i> within the
              context of the grid. Each instance of
              <i>IfcGridAxis</i> refers to the same instance of
              <i>IfcCurve</i> (here the subtype
              <i>IfcPolyline</i>) that is contained within the
              <i>IfcGeometricCurveSet</i> that represents the
              <i>IfcGrid</i>.</small>
            </p>
          </td>
        </tr>
      </tbody>
    </table>