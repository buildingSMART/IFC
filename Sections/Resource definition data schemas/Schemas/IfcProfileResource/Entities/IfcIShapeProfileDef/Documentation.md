﻿_IfcIShapeProfileDef_ defines a section profile that provides the defining parameters of an 'I' or 'H' section. The I-shape profile has values for its overall depth, width and its web and flange thicknesses. Additionally a fillet radius, flange edge radius, and flange slope may be given. This profile definition represents an I-section which is symmetrical about its major and minor axes; top and bottom flanges are equal and centred on the web.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Type of _FilletRadius_ relaxed to allow for zero radius. Attributes _FlangeEdgeRadius_ and _FlangeSlope_ added.

Figure 1 illustrates parameters of the I-shape profile definition.

<table>
<tr><td>
<table border="1" cellpadding="2" cellspacing="2" frame="border" width="100%">
  <tbody>
    <tr>
      <td width="420"><img src="../../../../../../figures/ifcishapeprofiledef-layout1.gif" alt="I-shape profile" border="0" height="300" width="400"></td>
      <td align="left" valign="top" width="100%">
      <p><u>Position</u>
      <br>
The parameterized
profile defines its own position coordinate system.
The underlying
coordinate system is defined by the swept area solid
that uses the profile definition. It is the xy plane of: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
by using offsets of the position location, the parameterized profile
can be positioned centric (using x,y offsets = 0.), or at any position
relative to the profile. Explicit coordinate offsets are used to define
cardinal points (e.g. upper-left bound).
      <p><u>Parameter</u>
      <br>
The parameterized profile
is defined by a set of parameter attributes, see attribute definition
below.</p>
      </td>
    </tr>
    <tr>
      <td width="420"><img src="../../../../../../figures/ifcishapeprofiledef-layout2.gif" alt="I shape with fillet" border="0" height="300" width="400"><br>
      <font size="-1">Note:
The black coordinate axes show the
underlying coordinate system of the swept surface or swept area solid</font></td>
      <td align="left" valign="top" width="100%">
      <p><u>Position</u>
      <br>
The profile is inserted into the underlying
coordinate system of the swept area solid by using the <em>Position</em>
attribute. In this example (cardinal point of lower left corner) the
attribute values of <em>IfcAxis2Placement2D</em>
are:</p>
      <blockquote>
        <p> <tt>Location
= IfcCartesianPoint(&lt;1/2
OverallWidth&gt;,&lt;1/2 OverallDepth&gt;)<br>
RefDirection = NIL (defaults to 1.,0.)</tt></p>
      </blockquote>
      <p><u>Parameter</u><br>
If the <em>FilletRadius</em>
is given, it is equally applied to all four corners created by the web
and flanges.</p>
      </td>
    </tr>
  </tbody>
</table>
</td></tr>
<tr><td><p class="figure">Figure 1 &mdash; I-shape profile</p></td></tr>
</table>
