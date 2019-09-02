**Definition
from IAI**: The _IfcAsymmetricIShapeProfileDef_ defines a section profile that provides the defining parameters of an asymmetric I-shaped section to be used by the swept area solid. The bottom flange is always wider than the top flange. Its parameters and orientation relative to the position coordinate system are according to the following illustration. The centre of the position coordinate system is in the profiles centre of the <span style="text-decoration: line-through;">gravity</span> bounding box.

The centre of gravity, if given, is located in x direction within the center of the bounding box, and in y-direction along the negative y axis, the offset value is given by the offset parameter<span style="font-style: italic;"> </span>_CentreOfGravityInY._

> <font size="-1">NOTE: The inherited
attributes </font><font size="-1">are used to
define:<br>
  </font><ul>
    <li><font size="-1"><i>OverallWidth -- </i></font><font size="-1"><i>BottomFlangeWidth</i></font></li>
    <li><font size="-1"><i>FlangeThickness</i>
-- </font><font size="-1"><i>BottomFlangeThickness</i></font></li>
    <li><font size="-1"><i>FilletRadius</i>
-- <i>BottomFlangeFilletRadius</i>.</font></li>
  </ul>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in Release IFC2x Edition 2.</font></small>  
>   
> <small><font color="#ff0000">IFC2x Edition 3 CHANGE&nbsp; All profile
origins are now in the center of the bounding box. The attribute <i>CentreOfGravityInY</i>
has been made OPTIONAL. Upward compatibility for file based exchange is
guaranteed.</font></small>

**Illustration**:

<table style="text-align: left; width: 100%;" border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td style="vertical-align: top; text-align: left; width: 420px;"><a href="drawings/IfcAsymmetricIShapeProfileDef.dwf"><span style="text-decoration: underline;"><img style="border: 0px solid ; width: 400px; height: 300px;" alt="asymmetric I shape profile" src="figures/IfcAsymmetricIShapeProfileDef.gif"></span></a></td>
      <td style="vertical-align: top; text-align: left;">
      <p><u>Position</u> <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of:</p>
      <ul>
        <li><i>IfcSweptAreaSolid.Position</i></li>
      </ul>
by using offsets of the position location,
the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile. Explicit coordinate offsets are used to define
cardinal points (e.g. upper-left bound).<span style="font-style: italic;"></span>
      <p><u>Parameter</u> <br>
The parameterized profile
is defined by a set of parameter attributes, see attribute definition
below.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Parameters of asymmetric I-shaped section definition