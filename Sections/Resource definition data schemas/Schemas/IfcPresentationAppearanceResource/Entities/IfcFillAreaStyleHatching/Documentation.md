**Definition
from ISO/CD 10303-46:1992**: The fill area style hatching defines a styled pattern of curves for hatching an annotation fill area or a surface.

**Definition
from IAI**: The _IfcFillAreaStyleHatching_ is used to define simple, vector-based hatching patterns, based on styled straight lines. The curve font, color and thickness is given by the _HatchLineAppearance_, the angle by the _HatchLineAngle_ and the distance to the next hatch line by _StartOfNextHatchLine_, being either an offset distance or a vector.

> <small>NOTE&nbsp;
If the hatch pattern involves two (potentially
crossing) rows of hatch lines, then two instances of <i>IfcFillAreaStyleHatching</i>
should be assigned to the <i>IfcFillAreaStyle</i>.
Both share the same
(virtual) point of origin of the hatching that is used by the reference
hatch line (or the <i>PointOfReferenceHatchLine</i>
if there is an
offset).</small>
> 


For better control of the hatching appearance, when using hatch lines with other fonts then continuous, the _PatternStart_ allows to offset the start of the curve font pattern along the reference hatch line (if not given, the _PatternStart_ is at zero distance from the virtual point of origin). If the reference hatch line does not go through the origin (of the virtual hatching coordinate system), it can be offset by using the&nbsp;_PatternStart&nbsp;_~~_PointOfReferenceHatchLine_.~~

> <small>NOTE&nbsp;
The coordinates of the <i>PatternStart </i><strike>and
the </strike><i><strike>PointOfReferenceHatchLine</strike>
</i>are
given relative to the assumed
0., 0. virtual point of origin at which the hatch pattern is later
positioned by the <i>FillStyleTarget</i>
point at <i>IfcAnnotationFillAreaOccurrence</i>.&nbsp;
The measure values are given in global drawing length units and apply
to the target plot scale for the scale depended representation
subcontext.</small>
> 
> <font color="#ff0000"><small>NOTE
&nbsp;The use of </small><small><i>PointOfReferenceHatchLine</i>
is deprecated.</small></font>
> 


**Illustration**

<table border="1" cellpadding="2" cellspacing="2" width="100%"> <tbody> <tr> <td align="left" valign="top" width="300"><img alt="hatch example 1" src="figures/ifcfillareastylehatching_fig1.gif" height="300" width="300"></td> <td align="left" valign="top"><small>Fig.1<br>
simple hatching given by using a curve font "continuous" at <i>HatchLineAppearance</i>.<br>
<br>
The distance of hatch lines is given by a positive length measure. The
angle (here 45' if measures in degree) is provided by <i>HatchLineAngle</i>.<br>
<br>
The <i>PatternStart</i> is
set to NIL ($) in this example.</small></td> <td align="left" valign="top" width="300"><img alt="hatch example 2" src="figures/ifcfillareastylehatching_fig2.gif" height="300" width="300"></td> <td align="left" valign="top"><small>Fig.
2<br>
hatching from figure 1 with using a different curve font at <i>HatchLineAppearance</i>.<br>
<br> </small><small>The
distance of hatch lines is given by a positive
length measure, therefore the font pattern start is at a point at the
next hatch line given by a vector being perpendicular to the point of
origin at the reference hatch line.<br> <br> </small><small>The
<i>PatternStart</i> is set to NIL ($) in this example.</small></td>
</tr> <tr> <td width="300"><img alt="hatch example 3" src="figures/ifcfillareastylehatching_fig3.gif" height="300" width="300"></td> <td align="left" valign="top"><small>Fig.
3<br>
hatching from figure 2 with using a vector to determine the pattern
start of the next hatch lines.<br> <br>
The pattern start is the beginning of the first visual curve font
pattern segment at <i>IfcCurveFont.
CurveFont</i>.<br> <br> </small><small>The
<i>PatternStart</i> is set to NIL ($) in this example.</small><br>
</td> <td width="300"><img alt="hatch example 4" src="figures/ifcfillareastylehatching_fig4.gif" height="300" width="300"></td> <td align="left" valign="top"><small>Fig.
4<br>
hatching from figure 3 where the pattern start is offset from the </small><small>point
of origin at the reference hatch line. I.e. the first visible curve
font pattern segment now does not start at the </small><small>point
of
origin at the reference hatch line.</small><small> </small><small></small><br>
<small><br> </small></td> </tr> <tr>
<td><img alt="hatch example 5" src="figures/ifcfillareastylehatching_fig5.gif" height="300" width="300"></td> <td align="left" valign="top"><small>Fig.
5<br>
hatching from figure 4 where the hatch pattern is shifted against the
underlying coordinate system</small><small>.<br> <br>
The point that is mapped to the insertion point of the <i>IfcAnnotationFillAreaOccurrence</i>
now has an x and y offset from the start of the reference hatch line.
I.e. the reference hatch line now does not go through the insertion
point of the hatching.<br> <br> <br> <br> </small></td>
<td valign="top"><img alt="fig 6" src="figures/ifcfillareastylehatching_fig6.gif" height="300" width="300"></td> <td valign="top"><small>Fig.
6<br>
use of <i>IfcFillAreaStyleHatching</i> attributes for two </small><small><i>IfcFillAreaStyleHatching</i>'s
within one <i>IfcFillAreaStyle</i>.<br> <br> </small><small>NOTE:
The <i>PatternStart</i> now displaces both the reference
hatch line from the point of origin and the start of the curve pattern.
This can be used e.g. when more then one <i>IfcFillAreaStyleHatching</i>
is used in an <i>IfcFillAreaStyle</i> in order to place
rows of hatch lines with an offset from each other.</small></td>
</tr> </tbody>
</table>

> <font color="#0000ff"><small>
NOTE&nbsp; Corresponding
STEP name: fill_area_style_hatching. Please refer to ISO/IS
10303-46:1994, p. 108 for the final definition of the formal standard.</small>
</font>

> <font #0000ff=""><small>HISTORY&nbsp;
New entity in
Release
IFC2x&nbsp;Edition 2.</small><br> </font><font color="#ff0000"><small>IFC2x
Edition 3 CHANGE&nbsp; The <i>IfcFillAreaStyleHatching</i>
has
been changed
by making the attributes PatternStart and PointOfReferenceHatchLine
OPTIONAL. The attribute <i>StartOfNextHatchLine</i>
has changed to a
SELECT with the additional choice of <i>IfcPositiveLengthMeasure</i>.
Upward compatibility for file based exchange is guaranteed. </small></font>
