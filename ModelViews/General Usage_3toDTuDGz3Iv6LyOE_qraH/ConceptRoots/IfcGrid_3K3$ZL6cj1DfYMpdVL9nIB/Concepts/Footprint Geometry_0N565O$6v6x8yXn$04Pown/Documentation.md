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
            <img src="../../../figures/ifcdesigngrid-layout1.gif" alt="design grid" border="0" height="300" width="400">
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
            <p class="figure">Figure 1 &mdash; Grid layout</p>
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
            <img src="../../../figures/ifcgrid-representation.png" alt="representation of a design grid" width="501" height="621" border="0">
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
            <p class="figure">Figure 2 &mdash; Grid representation</p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </tbody>
    </table>