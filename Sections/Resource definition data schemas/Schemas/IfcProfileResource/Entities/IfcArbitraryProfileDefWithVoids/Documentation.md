**Definition
from IAI**: The _IfcArbitraryProfileDefWithVoids_ defines an arbitrary closed two-dimensional profile with holes defined for the use for the swept area solid or a sectioned spine. It is given by an outer boundary and inner boundaries from with the solid the can be constructed.

> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC
Release 2x.</font>

**Informal
propositions**:

1. The outer curve and all inner curves shall be closed curves.
2. The outer curve shall enclose all inner curves.
3. No inner curve shall intersect with the outer curve or any other inner curve.
4. No inner curve may enclose another inner curve.

**Illustration**:

<table style="width: 100%;" border="1" cellpadding="2" cellspacing="2" frame="border">
  <tbody>
    <tr>
      <td align="left" valign="top" width="420"><a href="drawings/IfcArbitraryProfileDef-Layout2.dwf"><img src="figures/ifcarbitraryprofiledef-layout2.gif" alt="arbitrary profile with inner boundaries" border="0" height="300" width="400"></a></td>
      <td style="width: 100%; vertical-align: top; text-align: left;">
      <p><u>Position</u>
      <br>
The <i>OuterCurve</i>,
defined at the supertype <i>IfcArbitraryClosedProfileDef</i>
and the inner curves are defined in the same underlying coordinate
system. The common underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
      <p>or in case of sectioned
spines the xy plane of each list
member of <span style="font-style: italic;">IfcSectionedSpine.CrossSectionPositions</span></p>
      <p><span style="font-style: italic;"></span><u>Parameter</u>
      <br>
The <i>OuterCurve</i>
attribute defines a two dimensional closed
bounded curve, the <i>InnerCurves</i>
define a set of two dimensional
closed bounded curves.</p>
      </td>
    </tr>
  </tbody>
</table>

Table: Definition of arbitrary closed profile definition with voids