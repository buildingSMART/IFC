**Definition
from IAI**: The _IfcTrapeziumProfileDef_ defines a trapezium as the profile definition used by the swept surface geometry or the swept area solid. It is given by its Top X and Bottom X extent and its Y extent as well as by the offset of the Top X extend, and placed within the 2D position coordinate system, established by the _Position_ attribute. It is placed <font color="#ff0000">centric</font> within the position coordinate system, i.e. in the center of the bounding box.

> <font color="#0000ff" size="-1">HISTORY: New class
in IFC
Release 1.5. The use definition has changed in IFC Release 2x.</font>

**Illustration:**<table frame="border" width="100%">
  <tbody>
    <tr>
      <td width="420"><a href="drawings/IfcTrapeziumProfileDef-Layout1.dwf"><img src="figures/ifctrapeziumprofiledef-layout1.gif" alt="trapezium profile" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top" width="100%"><u>Position</u>
      <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept surface or swept area solid
that uses the profile definition. It is the xy plane of either:
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
The <i>IfcTrapeziumProfileDef</i>
is defined within the position
coordinate system, where the <i>BottomDim</i>
defines the length
measure for the bottom line (half along the positive x-axis) and the <i>YDim</i>
defines the length measure for the parallel distance of bottom and top
line (half along the positive y-axis). The top line starts with a
distance of <i>TopXOffset</i>
from [-BottomLine/2,YDim] (which can be
negative, zero, or positive) and has a length of <i>TopXDim</i>
along
the positive x-axis.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameter of trapezium profile definition