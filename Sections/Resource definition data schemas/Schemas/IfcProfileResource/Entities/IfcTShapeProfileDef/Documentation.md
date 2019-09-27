﻿_IfcTShapeProfileDef_ defines a section profile that provides the defining parameters of a T-shaped section to be used by the swept area solid. Its parameters and orientation relative to the position coordinate system are according to the following illustration. The centre of the position coordinate system is in the profile's centre of the bounding box.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; All profile origins are now in the center of the bounding box.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Type of _FilletRadius_, _FlangeEdgeRadius_, and _WebEdgeRadius_ relaxed to allow for zero radius. Trailing attribute _CentreOfGravityInY_ deleted, use respective property in _IfcExtendedProfileProperties_ instead.

Figure 1 illustrates parameters of the T-shape profile definition.

<table><tr><td>
<table border="1" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td width="420">
<img src="../../../../../../figures/ifctshapeprofiledef.gif" alt="T-shape profile" border="0" height="300" width="400">

      </td>
      <td valign="top">

<p><u>Position</u> <br>
The parameterized profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of:</p>
      <ul>
        <li><small>IfcSweptAreaSolid.Position</small></li>
      </ul>
<p>by using offsets of the position location, the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile.</p>

      </td>
    </tr>
  </tbody>
</table>
</td></tr>
<tr><td><p class="figure">Figure 1 &mdash; T-shape profile</p></td></tr>
</table>
