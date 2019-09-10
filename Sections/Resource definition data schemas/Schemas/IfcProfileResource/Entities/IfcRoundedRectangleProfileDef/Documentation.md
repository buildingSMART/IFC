**Definition
from IAI**: The _IfcRoundedRectangleProfileDef_ defines a rectangle with equally rounded corners as the profile definition used by the swept surface geometry or the swept area solid. It is given by the X extent, the Y extent, and the radius for the rounded corners, and placed within the 2D position coordinate system, established by the _Position_ attribute. It is placed <font color="#ff0000">centric</font> within the position coordinate system, i.e. in the center of the bounding box.

> <font color="#0000ff" size="-1">HISTORY: New class
in IFC
Release 2x</font>

> <font color="#ff0000" size="-1">IFC2x PLATFORM
CHANGE: The <i>IfcRoundedRectangleProfileDef</i>
is now subtyped from <i>IfcRectangleProfileDef</i>.
The <i>XDim</i>
and <i>YDim</i>
attributes have been removed (now inherited from
supertype).</font>

**Illustration**:  
<table frame="border" width="100%">
  <tbody>
    <tr>
      <td width="420"><a href="drawings/IfcRoundedRectangleProfileDef-Layout1.dwf"><img src="figures/ifcroundedrectangleprofiledef-layout1.gif" alt="rounded rectangle profile" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top" width="100%">
      <p><u>Position</u>
      <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept surface or swept area solid
that uses the profile definition. It is the xy plane of either: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
or in case of sectioned spines the xy plane of each list member of <span style="font-style: italic;">IfcSectionedSpine.CrossSectionPositions.</span>
      <br>
      <br>
By using offsets of the position location, the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile. Explicit coordinate offsets are used to define
cardinal points (e.g. upper-left bound).
      <p><u>Parameter</u>
      <br>
The <i>IfcRoundedRectangleProfileDef</i>
is defined within the
position coordinate system, where the <i>XDim</i>
defines the measure
for the length of the rectangle (half along the positive x-axis), the <i>YDim</i>
defines the length measure for the width of the rectangle (half along
the positive y-axis) and the <i>RoundingRadius</i>
defines the radius
of curvature in all four corners of the rectangle.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameter of rounded rectangle profile definition
