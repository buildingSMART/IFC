**Definition
from IAI**: The _IfcCircleProfileDef_ defines a circle as the profile definition used by the swept surface geometry or by the swept area solid. It is given by its _Radius_ attribute and placed within the 2D position coordinate system, established by the _Position_ attribute.

> <font color="#0000ff" size="-1">HISTORY: New class
in IFC
Release 1.5. </font>

**Illustration**:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" frame="border">
  <tbody>
    <tr>
      <td width="420"><a href="drawings/IfcCircleProfileDef-Layout1.dwf"><img src="figures/IfcCircleProfileDef-Layout1.gif" alt="circle profile" border="0" height="300" width="400"></a></td>
      <td style="width: 100%; vertical-align: top; text-align: left;">
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
The <i>Position</i>
attribute defines the 2D position coordinate
system of the circle.<br>
The <i>Radius</i>
attribute defines the radius of the circle.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameter for circle profile definition