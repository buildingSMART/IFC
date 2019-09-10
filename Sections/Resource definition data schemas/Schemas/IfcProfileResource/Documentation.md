___
## IfcProfileResource
The schema _IfcProfileResource_ defines the two dimensional profiles or cross sections, used to define geometric shape representations. Profile definitions are applied to:

* swept surfaces
* swept area solids
* sectioned spines

> <font color="#0000ff" size="-1">NOTE: Profile
definitions are not subtypes of geometric representation item and can
not be used directly to geometrically represent an object.</font>

Profiles can be used to either define a curve or an area. In case of a curve, only the boundary is in the domain of the profile definition, in case of an area the boundary and the inside is in the domain of the profile definition. A curve can be used for

* swept surfaces
* sectioned spines

and an area can be used for

* swept area solids
* sectioned spines

> <font color="#0000ff" size="-1">NOTE: The use of
profile definitions is the preferred way to define prismatic shapes to
represent products.</font>

The profile definition (_IfcProfileDef_) can be instantiated by the various subtypes. There are four different groups of profile definitions:

* parametrically defined profiles, these profiles are defined by a 2D position coordinate system and dimension parameters to generate a 2D form.
* explicitly defined profiles, these profiles are defined by a (single or multiple) 2D curve(s) defined in the parent coordinate system.
* derived profiles, these profiles are created by a Cartesian transformation of a parent profile.
* composite profiles, these profiles are compositions of other profiles

When used as the curve or area to be swept into a surface or solid, the 2D coordinate system of the profile is mapped into the xy plane of the 3D coordinate system of the swept surface (subtypes of _IfcSweptSurface_), the swept area solid (subtypes of _IfcSweptAreaSolid_), or the sectioned spine (_IfcSectionedSpine_). The extrusion direction is along the z axis of the 3D coordinate system (or an extrusion vector being not perpendicular to the z axis, or a rotation that has a tangent into the z axis at the point of origin).

> <font color="#0000ff" size="-1">NOTE: The use of
coordinate axes in IFC is not identical with the general convention for
the use of coordinate axes in structural analysis. The following
conversion should be used:</font>
> 


<table>
  <tbody>
    <tr valign="top">
      <td><a href="lexical/drawings/IfcProfileResource-CoordinateSystem.dwf"><img src="../../../../figures/ifcprofileresource-coordinatesystem.gif" alt="coordinates in IFC and structural" border="0" height="300" width="400"></a></td>
      <td>
      <table cellspacing="4">
        <tbody>
          <tr>
            <td><font color="#0000ff" size="-1">IFC axes<br>
convention</font></td>
            <td><font color="#0000ff" size="-1">structural analysis <br>
axes convention</font></td>
          </tr>
          <tr>
            <td><font color="#0000ff" size="-1">+X</font></td>
            <td><font color="#0000ff" size="-1">-Y</font></td>
          </tr>
          <tr>
            <td><font color="#0000ff" size="-1">+Y</font></td>
            <td><font color="#0000ff" size="-1">-Z</font></td>
          </tr>
          <tr>
            <td><font color="#0000ff" size="-1">+Z</font></td>
            <td><font color="#0000ff" size="-1">+X</font></td>
          </tr>
        </tbody>
      </table>
      </td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">HISTORY: New schema
in IFC 2x, definitions had been part of the <i>IfcGeometryResource</i>
in earlier IFC Releases.</font>