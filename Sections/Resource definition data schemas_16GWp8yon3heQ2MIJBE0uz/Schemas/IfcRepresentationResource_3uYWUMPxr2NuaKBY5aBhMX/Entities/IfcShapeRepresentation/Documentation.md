**Definition
from ISO/CD 10303-42:1992**: The shape representation is a specific kind of representation that represents a shape.

**Definition
from IAI**: The _IfcShapeRepresentation_ represents the concept of a particular geometric representation of a product or a product component within a specific geometric representation context. The inherited attribute _RepresentationType_ is used to define the geometric model used for the shape representation, the inherited attribute _RepresentationIdentifier_ is used to denote the part of the representation captured by the _IfcShapeRepresentation_ (e.g. Axis, Body, etc.).

Several representation types for shape representation are included as predefined types:

<table cellpadding="2" cellspacing="2"> <tbody><tr>
<td colspan="2" align="left" valign="top" width="20"><b>Curve2D</b></td> <td align="left" valign="top">2
dimensional curves </td> </tr> <tr> <td colspan="2" align="left" valign="top" width="20"><b>GeometricSet
</b></td> <td align="left" valign="top">points,
curves, surfaces (2 or 3 dimensional)</td> </tr> <tr>
<td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="20"><b>GeometricCurveSet</b></td>
<td align="left" valign="top">points,
curves (2 or 3 dimensional)</td> </tr> <tr> <td></td>
<td><b>Annotation2D</b></td> <td>points,
curves (2 or 3 dimensional), hatches and text (2 dimensional) </td>
</tr> <tr> <td colspan="2" align="left" valign="top" width="20"><b>SurfaceModel </b></td>
<td align="left" valign="top">face
based and shell based surface model</td> </tr> <tr>
<td colspan="2" align="left" valign="top" width="20"><b>SolidModel </b></td> <td align="left" valign="top">including
swept solid, Boolean results and Brep bodies<br>
more specific types are:</td> </tr> <tr> <td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>SweptSolid</b></td>
<td align="left" valign="top">swept
area solids, by extrusion and revolution</td> </tr> <tr>
<td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>Brep</b></td>
<td align="left" valign="top">faceted
Brep's with and without voids</td> </tr> <tr> <td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>CSG</b></td>
<td align="left" valign="top">Boolean
results of operations between solid models, half spaces and Boolean
results</td> </tr> <tr> <td align="left" valign="top" width="20">&nbsp;</td> <td align="left" valign="top" width="130"><b>Clipping</b></td>
<td align="left" valign="top">Boolean
differences between swept area solids, half spaces and Boolean results</td>
</tr> <tr> <td align="left" valign="top" width="20">&nbsp;</td> <td align="left" valign="top" width="130"><b>AdvancedSweptSolid</b></td>
<td align="left" valign="top">swept
area solids created by sweeping a profile along a directrix</td> </tr>
<tr> <td colspan="2" align="left" valign="top" width="20"><i>additional
types</i> </td> <td align="left" valign="top">some
additional representation types are given:</td> </tr> <tr>
<td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>BoundingBox</b></td>
<td align="left" valign="top">simplistic
3D representation by a bounding box</td> </tr> <tr>
<td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>SectionedSpine</b></td>
<td align="left" valign="top">cross
section based representation of a spine curve and planar cross
sections. It can represent a surface or a solid and the interpolations
of the between the cross sections is not defined</td> </tr>
<tr> <td align="left" valign="top" width="20">&nbsp;</td>
<td align="left" valign="top" width="130"><b>MappedRepresentation</b></td>
<td align="left" valign="top">representation
based on mapped item(s), referring to a representation map. Note: it
can
be seen as an inserted block reference. The shape representation of the
mapped item has a representation type declaring the type of its
representation items.</td> </tr> </tbody>
</table>

Table 1: string values for the inherited attribute '_RepresentationType_'.

> <small>NOTE&nbsp; The definition of
this entity relates to the STEP entity shape_representation. Please
refer to ISO/IS
10303-41:1994 for the final definition of the formal standard. </small>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 1.5. </font></small>