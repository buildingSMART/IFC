**Definition
from IAI**: The open profile _IfcArbitraryOpenProfileDef_ defines an arbitrary two-dimensional open profile for the use within the swept surface geometry. It is given by an open boundary from with the surface can be constructed.

> <font color="#0000ff" size="-1">HISTORY: New
entity&nbsp;
in IFC Release 2x.</font>

**Informal
proposition**:

1. The _Curve_ has to be an open curve.

**Illustration**:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" frame="border">
  <tbody>
    <tr>
      <td align="left" valign="top" width="420"><a href="drawings/IfcArbitraryProfileDef-Layout3.dwf"><img src="figures/IfcArbitraryProfileDef-Layout3.gif" alt="arbitrary profile without boundaries" border="0" height="300" width="400"></a></td>
      <td style="width: 100%; vertical-align: top; text-align: left;">
      <p><u>Position</u>
      <br>
The <i>Curve</i>
is defined in the underlying coordinate system. The
underlying
coordinate system is defined by the swept surface that uses the profile
definition. It is the xy plane of: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
      </ul>
      <p><u>Parameter</u>
      <br>
The <span style="font-style: italic;">Curve
      </span>attribute defines
a two dimensional open bounded curve.&nbsp;</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Definition of arbitrary open profile definition