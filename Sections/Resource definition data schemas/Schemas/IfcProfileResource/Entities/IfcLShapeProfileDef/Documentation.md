**Definition
from IAI**: The _IfcLShapeProfileDef_ defines a section profile that provides the defining parameters of an L-shaped section (equilateral L profiles are also covered by this entity) to be used by the swept area solid. Its parameters and orientation relative to the position coordinate system are according to the following illustration. The shorter leg has the same direction as the positive x-axis, the longer or equal leg the same as the positive y-axis. The centre of the position coordinate system is in the profiles centre of the ~~gravity~~ bounding box.

The centre of gravity, if given, is located in x direction along the negative x axis, the offset value is given by the offset parameter _CentreOfGravityInX_, and in y-direction along the negative y axis, the offset value is given by the offset parameter _CentreOfGravityInY._

> <small><font color="#0000ff">HISTORY&nbsp;
New entity
in Release IFC2x Edition 2.</font></small>

> <small><font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; All profile
origins are now in the center of the bounding box. The attribute <i>CentreOfGravityInY</i>
has been made OPTIONAL. Upward compatibility for file based exchange is
guaranteed.</font></small>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td align="left" valign="top" width="420"><a href="drawings/IfcLShapeProfileDef_Layout1.dwf"><img alt="non equal sided L-shape" src="figures/ifclshapeprofiledef_layout1.gif" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
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
    <tr>
      <td><a href="drawings/IfcLShapeProfileDef_Layout2.dwf"><img alt="equal sided L-shape" src="figures/ifclshapeprofiledef_layout2.gif" border="0" height="300" width="400"></a><br>
      <font size="-1">Note:
The black coordinate axes show the
underlying coordinate system of the swept surface or swept area solid</font></td>
      <td align="left" valign="top">
      <p><u>Position</u> <br>
The profile is inserted into the underlying
coordinate system of the swept area solid by using the <i>Position</i>
attribute. In this example (cardinal point of gravity) the
attribute values of <i>IfcAxis2Placement2D</i>
are:</p>
      <blockquote>
        <p> <tt>Location
=
IfcCartesianPoint(&lt;CentreOfGravityInX&gt;,&lt;</tt><tt>CentreOfGravityInY</tt><tt>&gt;)<br>
RefDirection = NIL (defaults to 1.,0.)</tt></p>
      </blockquote>
      <p><font size="-1">Note: if the values of <i>CentreOfGravityInX</i>
and <i>CentreOfGravityInY</i>
are given, they are already negative
values, since the shift of the centre of gravity is into the negative X
and negative Y axis.</font></p>
      <p><u>Parameter</u><br>
If the <i>Width</i>
parameter is not given, it defaults to the value
of Depth, therefore an equal sided L-shape profile is created, if the <i>LegSlope</i>
parameter is not given, both legs have parallel edges.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameters of&nbsp; equal-sided and non-equal sided L-shaped section definition