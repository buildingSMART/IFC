The _IfcUShapeProfileDef_ defines a section profile that provides the defining parameters of a U-shape (channel) section to be used by the swept area solid. Its parameters and orientation relative to the position coordinate system are according to the following illustration. The centre of the position coordinate system is in the\^profiles centre of the ~~gravity~~ bounding box.

The centre of gravity, if given, is located in y direction within the center of the bounding box, and in x-direction along the negative x axis, the offset value is given by the offset parameter CentreOfGravityInX.

> <font color="#0000ff"><small>HISTORY&nbsp;
New entity in
Release IFC2x Edition 2.</small>
  </font>

> <small><font color="#ff0000">IFC2x
Edition 3
CHANGE&nbsp; All profile
origins are now in the center of the bounding box. The attribute <i>CentreOfGravityInX</i>
has been made
OPTIONAL. Upward compatibility for file based exchange is guaranteed.</font></small>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td valign="top" width="420"><a href="drawings/IfcUShapeProfileDef.dwf"><img src="figures/IfcUShapeProfileDef.gif" alt="U-shape profile" border="0" height="300" width="400"></a></td>
      <td valign="top">
      <p><u>Position</u> <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of:</p>
      <ul>
        <li><i>IfcSweptAreaSolid.Position</i></li>
      </ul>
by using offsets of the position location, the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile. Explicit coordinate offsets are used to define
cardinal points (e.g. upper-left bound).
      <p><u>Parameter</u> <br>
The parameterized profile
is defined by a set of parameter attributes, see attribute definition
below.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameters of U-shape profile definition