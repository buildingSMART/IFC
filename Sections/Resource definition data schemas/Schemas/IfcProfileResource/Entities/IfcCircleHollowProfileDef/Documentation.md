**Definition
from IAI**: The _IfcCircleHollowProfileDef_ defines a section profile that provides the defining parameters of a circular hollow section (tube) to be used by the swept area solid. Its parameters and orientation relative to the position coordinate system are according to the following illustration.The centre of the position coordinate system is in the profile's centre of the bounding box (for symmetric profiles identical with the centre of gravity).

> <font color="#0000ff" size="-1">HISTORY: New entity
in
Release IFC2x Edition 2.</font>

**Illustration**:

<table style="text-align: left; width: 100%;" border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td style="vertical-align: top; text-align: left; width: 420px;"><a href="drawings/IfcCircleHollowProfileDef.dwf"><img src="figures/ifccirclehollowprofiledef.gif" alt="CHS-shape profile" border="0" height="300" width="400"></a></td>
      <td style="vertical-align: top; text-align: left;">
      <p><u>Position</u>
      <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of:</p>
      <ul>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
by using offsets of the position location, the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile. Explicit coordinate offsets are used to define
cardinal points (e.g. upper-left bound).<span style="font-style: italic;"></span>
      <p><u>Parameter</u>
      <br>
The parameterized profile
is defined by a set of parameter attributes, see attribute definition
below.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameters of circular hollow profile definition
