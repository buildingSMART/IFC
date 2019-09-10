The&nbsp;_IfcVirtualGridIntersection_ defines the derived location of the intersection between two grid axes. Offset values may be given to set an offset distance to the grid axis for the calculation of the virtual grid intersection.

The two intersecting axes (_IntersectingAxes_) define the intersection point, which exact location (in terms of the Cartesian point representing the intersection) has to be calculated from the geometric representation of the two participating curves.

Offset values may be given (_OffsetDistances_). If given, the position within the list of _OffsetDistances_ corresponds with the position within the list of _IntersectingAxes_. Therefore:

* _OffsetDistances[1]_ sets the offset to _IntersectingAxes[1]_, 
* _OffsetDistances[2]_ sets the offset to _IntersectingAxes[2]_, and
* _OffsetDistances[3]_ sets the offset to the virtual intersection in direction of the orientation of the cross product of _IntersectingAxes[1]_ and the orthogonal complement of the _IntersectingAxes[1]_ (which is the positive or negative direction of the z axis of the design grid position).

> <font color="#0000ff" size="-1">HISTORY:
New entity in IFC Release 1.5. The entity name was changed from
IfcConstraintRelIntersection in IFC Release 2x.</font>

****Geometry use definitions**:**

The following figures explain the usage of the _OffsetDistances_ and _IntersectingAxes_ attributes.

<table cellpadding="2" cellspacing="2">
  <tbody>
    <tr valign="top">
      <td align="left" valign="top"><a href="drawings/IfcVirtualGridIntersection-Layout1.dwf"><img src="figures/ifcvirtualgridintersection-layout1.gif" alt="2D offsets" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">Two offset
distances given, the virtual intersection is defined in the xy plane of
the grid axis placement.</td>
    </tr>
    <tr valign="top">
      <td align="left" valign="top"><a href="drawings/IfcVirtualGridIntersection-Layout2.dwf"><img src="figures/ifcvirtualgridintersection-layout2.gif" alt="3D offsets" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">Three offset
distances given, the virtual intersection is defined by an offset (in
direction of the z-axis of the design grid placement) to the virtual
intersection in the xy plane of the grid axis placement.</td>
    </tr>
  </tbody>
</table>

The distance of the offset curve (_OffsetDistances[n]_) is measured from the basis curve. The distance may be positive, negative or zero. A positive value of distance defines an offset in the direction which is normal to the curve in the sense of an anti-clockwise rotation through 90 degrees from the tangent vector T at the given point. (This is in the direction of orthogonal complement(T).) This can be reverted by the _SameSense_ attribute at _IfcGridAxis_ which may switch the sense of the _AxisCurve_.

_Illustration_

<table cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td align="left" valign="top" width="320"><img src="figures/ifcvirtualgridintersection-offset1.gif" alt="offset direction" border="0" height="211" width="306"></td>
      <td align="left" valign="top"><u>example
of a negative offset</u>
      <ul>
        <li><i>IntersectingAxes[1].AxisCurve</i> is
an <i>IfcTrimmedCurve</i> with an <i>IfcCircle</i>
as <i>BasisCurve</i> and <i>SenseAgreement</i>
= TRUE. </li>
        <li><i>IntersectingAxes[1].SameSense</i> =
TRUE.</li>
        <li><i>OffsetDistances[1]</i> is a negative
length measure</li>
      </ul>
the figure shows the side of the offset.</td>
    </tr>
  </tbody>
</table>
