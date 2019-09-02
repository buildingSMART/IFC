**Definition
from IAI**: The closed profile _IfcArbitraryClosedProfileDef_ defines an arbitrary two-dimensional profile for the use within the swept surface geometry, the swept area solid or a sectioned spine. It is given by an outer boundary from which the surface or solid can be constructed.

> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC Release 1.5. Entity has been renamed from <span style="font-style: italic;">IfcArbitraryProfileDef</span>
in IFC Release 2x.</font>

**Informal
proposition**:

1. The _OuterCurve_ has to be a closed curve.
2. The _OuterCurve_ shall not intersect.

**Illustration**:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" frame="border">
  <tbody>
    <tr>
      <td align="left" valign="top" width="420"><a href="drawings/IfcArbitraryProfileDef-Layout1.dwf"><img src="figures/IfcArbitraryProfileDef-Layout1.gif" alt="arbitrary profile without boundaries" border="0" height="300" width="400"></a></td>
      <td style="width: 100%; vertical-align: top; text-align: left;">
      <p><u>Position</u>
      <br>
The <i>OuterCurve</i>
is defined in the underlying coordinate system. The underlying
coordinate system is defined by the swept surface or swept area solid
that uses the profile definition. It is the xy plane of either:</p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
or in case of sectioned spines the xy plane of each list member of <span style="font-style: italic;">IfcSectionedSpine.CrossSectionPositions</span>
      <p><u>Parameter</u>
      <br>
The <i>OuterCurve</i>
attribute defines a two dimensional closed bounded curve.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Definition of arbitrary closed profile definition