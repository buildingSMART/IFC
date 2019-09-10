**Definition
from IAI**: The _IfcEllipseProfileDef_ defines an ellipse as the profile definition used by the swept surface geometry or the swept area solid. It is given by its semi axis attributes and placed within the 2D position coordinate system, established by the _Position_ attribute.

> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC
Release 2x </font>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" frame="border" width="100%">
  <tbody>
    <tr>
      <td width="420"><a href="drawings/IfcEllipseProfileDef-Layout1.dwf"><img src="figures/ifcellipseprofiledef-layout1.gif" alt="ellipse profile" border="0" height="300" width="400"></a></td>
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
The location of the position coordinate system defines the center of
the ellipse. The <i>SemiAxis1</i>
attribute defines the first radius
of the ellipse in the direction of the x axis, the <i>SemiAxis2</i>
attribute defines the second radius of the ellipse in the direction of
the y axis.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameter for ellipse profile definition

> <font size="-1">NOTE: The semi axes of the ellipse are
rectangular to each other by definition.</font>