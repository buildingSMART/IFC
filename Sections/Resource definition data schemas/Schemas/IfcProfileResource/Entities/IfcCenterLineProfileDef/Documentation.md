The profile _IfcCenterLineProfileDef_ defines an arbitrary two-dimensional open, not self intersecting profile for the use within the swept solid geometry. It is given by an area defined by applying a constant thickness to a centerline, generating an area from which the solid can be constructed.

> <small><font color="#0000ff">HISTORY&nbsp;
New entity
in IFC2x Edition 3.</font></small>

**Informal proposition**:

1. The _Curve_ has to be an open curve.
2. The _Curve_ has to be a non-intersecting curve.

**Illustration**:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" frame="border">
  <tbody>
    <tr>
      <td align="left" valign="top" width="420"><a href="drawings/IfcArbitraryProfileDef-Layout4.dwf"><img alt="center line" src="figures/ifcarbitraryprofiledef-layout4.gif" border="0" height="300" width="400"></a><a href="drawings/IfcArbitraryProfileDef-Layout3.dwf"><br>
      </a></td>
      <td style="width: 100%; vertical-align: top; text-align: left;">
      <p><u>Position</u> <br>
The <i>Curve</i> is defined in the underlying coordinate
system. The
underlying
coordinate system is defined by the swept surface that uses the profile
definition. It is the xy plane of: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
      </ul>
      <p><u>Parameter</u> <br>
The <span style="font-style: italic;">Curve </span>attribute
defines
a two dimensional open bounded curve. The <i>Thickness</i>
attribute
defines a constant thickness along the curve.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Definition of center line profile definition