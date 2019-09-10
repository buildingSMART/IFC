**Definition
from IAI**: The _IfcCompositeProfileDef_ defines the profile by composition of other profiles. The composition is given by a set of at least two other profile definitions. Any profile definition (except for another composite profile) can be used to construct the composite.

> <font color="#0000ff" size="-1">HISTORY New entity
in IFC Release
2x.</font>
> 


**Illustration**:

<table border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr valign="top">
      <td style="vertical-align: top; text-align: left; width: 400px;"><a href="drawings/IfcCompositeProfileDef-Layout1.dwf"><img src="figures/ifccompositeprofiledef-layout1.gif" alt="composite" border="0" height="300" width="400"></a><br>
      <br>
      <font size="-1">Note:
The black coordinate axes show the
underlying coordinate system of the swept surface or swept area solid</font></td>
      <td style="vertical-align: top; text-align: left;">
      <p><u>Position</u>
      <br>
The <i>IfcCompositeProfileDef</i>
does not define an own position coordinate system, it is directly
defined in the underlying coordinate system. The underlying
coordinate system is defined by the swept surface or swept area solid
that uses the profile definition. It is the xy plane of either:</p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
or in case of sectioned spines the xy plane of each list member of <span style="font-style: italic;">IfcSectionedSpine.CrossSectionPositions<br>
      </span>
      <p><u>Parameter</u>
      <br>
The <i>IfcCompositeProfileDef</i>
is defined using other profile
definitions. Those other profile definitions are directly inserted into
the underlying coordinate system.</p>
      <ul>
        <li>In case of
parameterized profile definitions, the <i>Position</i>
attribute of those standard profiles is used to place the profiles
relatively to each other.</li>
        <li>In case of arbitrary
profile definitions, each Cartesian
coordinate is given directly within the underlying coordinate system.</li>
      </ul>
      </td>
    </tr>
  </tbody>
</table>

Table: Definition of composite profile definition
