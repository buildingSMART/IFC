_IfcGrid_ ia a planar design grid defined in 3D space used as an aid in locating structural and design elements. The position of the grid (_ObjectPlacement_) is defined by a 3D coordinate system (and thereby the design grid can be used in plan, section or in any position relative to the world coordinate system). The position can be relative to the object placement of other products or grids. The XY plane of the 3D coordinate system is used to place the grid axes, which are 2D curves (for example, line, circle, arc, polyline).

The inherited attributes _Name_ and _Description_ can be used to define a descriptive name of the grid and to indicate the grid's purpose. A grid is defined by (normally) two, or (in case of a triangular grid) three lists of grid axes. The following figures shows some examples.

A grid may support a rectangular layout as shown in Figure 1, a radial layout as shown in Figure 2, or a triangular layout as shown in Figure 3.

> NOTE&nbsp; The _PredefinedType_ denotes the type of grid that is represented by _IfcGrid_. The instantiation of _IfcGridAxis_'s has to agree to the _PredefinedType_, if provided.

> NOTE&nbsp; The grid axes, defined within the design grid, are those elements to which project objects will be placed relatively using the _IfcGridPlacement_.

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td width="320">
            <img src="../../../figures/IfcDesignGrid-Type1.gif" alt="1" border="0" height="211" width="306">
          </td>
          <td width="320">
            <img src="../../../figures/IfcDesignGrid-Type2.gif" alt="2" border="0" height="211" width="306">
          </td>
          <td width="320">
            <img src="../../../figures/IfcDesignGrid-Type3.gif" alt="3" border="0" height="211" width="306">
          </td>
        </tr>
        <tr>
          <td width="320">
            <p class="figure">Figure 1 &mdash; Grid rectangular layout</p>
          </td>
          <td width="320">
            <p class="figure">Figure 2 &mdash; Grid radial layout</p>
          </td>
          <td width="320">
            <p class="figure">Figure 3 &mdash; Grid triangular layout</p>
          </td>
        </tr>
      </tbody>
    </table>

> HISTORY&nbsp; New entity in IFC1.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _PredefinedType_ has been added at the end of the attribute list.

&nbsp;

{ .spec-head}
Informal Propositions:

<table summary="IP">
      <tr>
        <td width="640">
          <ol>
            <li>Grid axes, which are referenced in different lists
            of axes (UAxes, VAxes, WAxes) shall not be parallel.
            </li>
            <li>Grid axes should be defined such as there are no
            two grid axes which intersect twice (see Figure 189).
            </li>
          </ol>
          <blockquote class="note">
            NOTE&nbsp; Left side: ambiguous intersections A1 and
            A2, a grid containing such grid axes is not a valid
            design grid;&nbsp; Right side: the conflict can be
            resolved by splitting one grid axis in a way, such as
            no ambiguous intersections exist.
          </blockquote>
        </td>
        <td align="right" valign="top" width="320">
          <img src="../../../figures/IfcDesignGrid-IP2.gif" alt="IP2" border="0" height="97" width="306">
          <p class="figure">Figure 4 &mdash; Grid intersections</p>
        </td>
      </tr>
    </table>

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcgrid.htm)

{ .use-head}
Product Placement

The [Product Placement](../../templates/product-placement.htm) concept applies to this entity.

The local placement for _IfcGrid_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

  
  
{ .use-head}
FootPrint Geometry

The [FootPrint Geometry](../../templates/footprint-geometry.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcGrid FootPrint Geometry</p></td></tr></table>

The 2D geometric representation of _IfcGrid_ is defined using the 'GeometricCurveSet' geometry. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet' . 

The following constraints apply to the 2D representation:

* The _IfcGeometricCurveSet_ shall be an (and the only) _Item_ of the _IfcShapeRepresentation_. It should contain an _IfcGeometricCurveSet_ containing subtypes of _IfcCurve_, each representing a grid axis. Applicable subtypes of _IfcCurve_ are: _IfcPolyline_, _IfcCircle_, _IfcTrimmedCurve_ (based on _BaseCurve_ referencing _IfcLine_ or _IfcCircle_), and _IfcOffsetCurve2D_. 
* Each subtype of _IfcCurve_ may have a curve style assigned, using _IfcStyledItem_ referencing _IfcCurveStyle_. 
* Optionally the grid axis labels may be added as _IfcTextLiteral_, and they may have text styles assigned, using _IfcStyledItem_ referencing _IfcTextStyle_. 

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td width="510">
            <img src="../../../figures/IfcDesignGrid-Layout1.gif" alt="design grid" border="0" height="300" width="400">
          </td>
          <td>
            <blockquote>
              As shown in Figure 31, the <em>IfcGrid</em> defines a
              placement coordinate system using the
              <em>ObjectPlacement</em>. The XY plane of the
              coordinate system is used to place the 2D grid axes.
              The <em>Representation</em> of <em>IfcGrid</em> is
              defined using <em>IfcProductRepresentation</em>,
              referencing an <em>IfcShapeRepresentation</em>, that
              includes&nbsp;<em>IfcGeometricCurveSet</em> as
              <em>Items</em>. All grid axes are added as
              <em>IfcPolyline</em> to the
              <em>IfcGeometricCurveSet</em>.
            </blockquote>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">Figure 5 &mdash; Grid layout</p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </tbody>
    </table>

&nbsp;

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr>
          <td width="510">
            <img src="../../../figures/IfcGrid-Representation.png" alt="representation of a design grid" width="501" height="621" border="0">
          </td>
          <td>
            <blockquote>
              As shown in Figure 32, the attributes <em>UAxes</em>
              and <em>VAxes</em> define lists of <em>IfcGridAxis</em>
              within the context of the&nbsp;grid. Each instance of
              <em>IfcGridAxis</em> refers to the same instance of
              <em>IfcCurve</em> (here the subtype <em>IfcPolyline</em>)
              that is contained within the
              <em>IfcGeometricCurveSet</em> that represents the
              <em>IfcGrid</em>.
            </blockquote>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">Figure 6 &mdash; Grid representation</p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </tbody>
    </table>