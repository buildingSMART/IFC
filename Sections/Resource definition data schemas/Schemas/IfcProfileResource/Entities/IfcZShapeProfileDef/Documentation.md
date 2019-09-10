**Definition
from IAI**: The _IfcZShapeProfileDef_ defines a section profile that provides the defining parameters of a Z-shape section to be used by the swept area solid. Its parameters and orientation relative to the position coordinate system are according to the following illustration. The centre of the position coordinate system is in the profiles centre of the <span style="text-decoration: line-through;">gravity</span> bounding box.

> <font color="#0000ff" size="-1">HISTORY: New entity
in
Release IFC2x Edition 2.</font>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td width="420"><a href="drawings/IfcZShapeProfileDef.dwf"><img src="figures/ifczshapeprofiledef.gif" alt="Z-shape profile" border="0" height="300" width="400"></a></td>
      <td valign="top">
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

Table: Parameters of Z-shape profile definition