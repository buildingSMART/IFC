**Definition
from IAI**: The _IfcProfileDef_ is the supertype of all definitions of standard and arbitrary profiles within IFC. It is used to define a standard set of commonly used profiles by their parameters or by their explicit curve geometry. Those profile definitions are used within the geometry and geometric model resource to create either swept surfaces, swept area solids, or sectioned spines.

The purpose of the profile definition within the swept surfaces or swept area solids is to define a uniform cross section being swept:

* along a line (extrusion) using _IfcSurfaceOfLinearExtrusion_ or _IfcExtrudedAreaSolid_
* along a circular arc (revolution) using _IfcSurfaceOfRevolution_ or _IfcRevolvedAreaSolid_
* along a directrix lying on a reference surface using _IfcSurfaceCurveSweptAreaSolid_

The purpose fo the profile definition within the sectioned spine is to define a varying cross sections at several positions along a spine curve. The subtype _IfcDerivedProfileDef_ is particularly suited to provide the consecutive profiles to be based on transformations of the start profile and thus maintaining the identity of vertices and edges.

> <font size="-1">NOTE: Subtypes of the <i>IfcProfileDef</i>
contain parameterized profiles (as subtypes of <i>IfcParameterizedProfileDef</i>)
which establish their own 2D position coordinate system, profiles given
by explicit curve geometry (either open or closed profiles) and two
special types for composite profiles and derived profiles, based on a
2D Cartesian transformation.</font>

* Parameterized profiles are 2D primitives, which are used within the industry to describe cross sections by a description of its parameters.    
* Arbitrary profiles are cross sections defined by an outer boundary as bounded curve, which may also include holes, defined by inner boundaries.    
* Derived profiles, based on a transformation of a parent profile, are also part of the profile definitions available.    
* In addition composite profiles can be defined, which include two or more profile definitions to define the resulting profile.

An _IfcProfileDef_ is treated as bounded area if it is used within swept area solids. In this case, the inside of the profile is part of the profile. The attribute _ProfileType_ is set to AREA. An _IfcProfileDef_ is treated as a curve if it is used within swept surfaces. In this case, the inside of the profile (if the curve is closed) is not part of the profile. The attribute _ProfileType_ is set to CURVE. The optional attribute _ProfileName_ can be used to designate a standard profile type as e.g. given in profile tables for steel profiles.

> <font color="#0000ff" size="-1">HISTORY: New class
in IFC Release 1.5, the capabilities have been extended in IFC Release
2x. Profiles can now support swept surfaces and swept area solids with
inner boundaries. It had been renamed from IfcAttDrivenProfileDef.<br>
  </font>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" frame="border" width="100%">
  <tbody>
    <tr valign="top">
      <td align="left" valign="top" width="420"><a href="drawings/IfcProfileDef-Layout1.dwf"><img src="figures/IfcProfileDef-Layout1.gif" alt="Example of standard profile definition" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
      <p><u>Position</u>
      <br>
The <i>IfcProfileDef</i>
is defined within the underlying
coordinate system thtt is defined by the swept surface or swept area
solid
that uses the profile definition. It is the xy plane of either: </p>
      <ul>
        <li style="font-style: italic;">IfcSweptSurface.Position</li>
        <li style="font-style: italic;">IfcSweptAreaSolid.Position</li>
      </ul>
or in case of sectioned spines the xy plane of each list member of <span style="font-style: italic;">IfcSectionedSpine.CrossSectionPositions</span>
      <p><font size="-1">Note: The parameterized profile definition
defines a 2D position coordinate system, relative to the underlying
coordinate system of the <i>IfcProfileDef</i>.</font></p>
      </td>
    </tr>
    <tr>
      <td width="420"><a href="drawings/IfcProfileDef-Layout5.dwf"><img src="figures/IfcProfileDef-Layout5.gif" alt="use within swept area solids" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
      <p><u>Sweeping</u></p>
      <p>In the later use of the <i>IfcProfileDef</i>
within the swept surface or swept area solid,&nbsp; e.g. the <i>IfcExtrudedAreaSolid</i>
(here used as an example), the profile boundaries (here based on the 2D
position coordinate system of <i>IfcParameterizedProfileDef</i>)
are placed within the xy plane of the 3D position coordinate system of
the swept surface or swept area solid. <br>
      </p>
      <p>The profile is inserted
into the underlying coordinate system either:</p>
      <ul>
        <li>directly in case of
using <i>IfcArbitraryClosedProfileDef</i>
and <i>IfcArbitraryOpenProfileDef</i>,</li>
        <li>through an
intermediate position coordinate system in case of using <i>IfcParameterizedProfileDef</i>.</li>
        <li>through an 2D
Cartesian transformation operator (applied directly to the curve
position when using arbitrary profile definitions, or applied to the
position coordinate system when using parameterized profile
definitions) in case of using <i>IfcDerivedProfileDef</i>.</li>
        <li>when using <i>IfcCompositeProfileDef</i>
the insertion depends on the subtype of the included sub-profiles.<br>
        </li>
      </ul>
      </td>
    </tr>
  </tbody>
</table>


Table: Use of parameterized profiles within the swept area solid
**Use
cases**:


Results of the different usage of the _ProfileType_
attribute are demonstrated here. The _ProfileType_
defines whether the inside (the bounded area) is part of the profile
definition (Area) or not (Curve).
<table border="1" cellpadding="2" cellspacing="2" frame="border" width="100%">
  <tbody>
    <tr>
      <td width="420"><img src="figures/IfcProfileDef-Layout3.gif" alt="area without thickness" height="225" width="300"><br>
ProfileType = AREA</td>
      <td align="left" valign="top"><img src="figures/IfcProfileDef-Layout4.gif" alt="closed curve" height="225" width="300"><br>
ProfileType = CURVE </td>
    </tr>
  </tbody>
</table>

Table: Resulting area or curve depending on _ProfileType_