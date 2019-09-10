The polygonal bounded half space is a special subtype of a half space solid, where the material of the half space used in Boolean expressions is bounded by a polygonal boundary. <font color="#0000ff">The base
surface of the half space is positioned by its normal relativeto the
object coordinate system
(as defined at the supertype <i>IfcHalfSpaceSolid</i>),&nbsp;and
its polygonal (with or without arc segments) boundary is defined in the
XY plane of the position
coordinate system established by the <i>Position</i>
attribute, the subtraction body is extruded perpendicular to the XY
plane of the position coordinate system, i.e. into the direction of the
positive Z axis defined by the <i>Position</i> attribute</font>.

The boundary is defined by a 2 dimensional polyline <font color="#0000ff">(or 2 dimensional composite curve,
consisting of straight segments and circular arc segments)</font> within the XY plane of the position coordinate system. The side of the surface which is in the half space is determined by the surface normal and the agreement flag. If the agreement flag is TRUE, then the subset is the one the normal points away from. If the agreement flag is FALSE, then the subset is the one the normal points into.

> <small>NOTE&nbsp; A polygonal
bounded half
space is not a subtype of <i>IfcSolidModel</i>,
half space solids are only useful as operands in Boolean expressions.</small>
> 


> <small><font color="#0000ff">HISTORY&nbsp;
New class in IFC Release 2x </font></small>
> 


**Informal propositions**:

<ol>
  <li>The <i>IfcPolyline</i> <font color="#0000ff">or the <i>IfcCompositeCurve</i></font>
providing the <i>PolygonalBoundary</i>
shall be closed.</li>
  <li>If the <i>PolygonalBoundary</i>
is given by an <i>IfcCompositeCurve</i>, it shall only
have&nbsp;<font color="#0000ff"><i><font color="#000000">I</font><font color="#000000">fcCompositeCurveSegment</font></i><font color="#000000">'s of type <i>IfcPolyline</i>,
or <i>IfcTrimmedCurve</i> (having a <i>BasisCurve</i>
of type <i>IfcLine</i>, or <i>IfcCircle</i>)</font></font></li>
</ol>
**Illustration**:

<table border="0" cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td width="650"><a href="drawings/IfcPolygonalBoundedHalfSpace-Layout1.dwf"><img alt="polygonal bounded halfspace" src="figures/ifcpolygonalboundedhalfspace-layout1.png" border="0" height="480" width="640"></a></td>
      <td align="left" valign="top"><small><u>black
coordinates</u><br>
      </small>
      <ul>
        <li><small>Object coordinate system (usually
provided by <i>IfcLocalPlacement</i>)</small></li>
      </ul>
      <small><br>
      <u>green coordinates</u><br>
      </small>
      <ul>
        <li><small>Position coordinate system, the <i>PolygonalBoundary</i>
is given within this coordinate system. It is provided by <i>IfcPolygonalBoundedHalfSpace.Position</i>.
This coordinate system is relative to the object coordinate system. The
extrusion direction of the subtraction body is the positve Z axis.</small></li>
      </ul>
      <small><u>red coordinates</u><br>
      </small>
      <ul>
        <li><small>Normal of the plane. It is provided by
the <i>BaseSurface</i>, i.e.&nbsp; <i>IfcSurface.Position</i>.
This normal is also relative to the object coordinate system.</small></li>
      </ul>
      </td>
    </tr>
    <tr>
      <td colspan="2" rowspan="1" align="left" valign="top">
      <p><font size="-1"><u>Purpose</u><br>
The polygonal bounded half space is used to limit the volume of the
half space in Boolean difference expressions. Only the part that is
defined by a theoretical intersection between the half space solid and
an extruded area solid, defined by extruding the polygonal boundary, is
used for Boolean expressions.</font></p>
      <p><font size="-1"><u>Parameter</u><br>
The <i>PolygonalBoundary</i> defines the 2D polyline which
bounds the effectiveness of the half space in Boolean expressions. The <i>BaseSurface</i>
is defined by a plane, and the normal of the plane together with the <i>AgreementFlag</i>
defines the side of the material of the half space.</font></p>
      </td>
    </tr>
  </tbody>
</table>
