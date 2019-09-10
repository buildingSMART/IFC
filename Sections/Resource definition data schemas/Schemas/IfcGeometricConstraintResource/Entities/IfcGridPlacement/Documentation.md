The _IfcGridPlacement_ provides a specialization of _IfcObjectPlacement_ in which the placement and axis direction of the object coordinate system is defined by a reference to the design grid as defined in _IfcGrid_.

The location of the object coordinate system is given by the attribute _PlacementLocation_. The axis direction (of x-axis) of the object coordinate system is given:

* by the tangent of the first grid axis (_PlacementLocation.IntersectingAxes[1]_) at the virtual intersection (maybe using the offset curve, if _PlacementLocation.OffsetDistances_ is given) in case that the _PlacementRefDirection_ is not given,
* by the tangent between the virtual grid intersection of _PlacementLocation_ and the virtual grid intersection of _PlacementRefDirection_ in case that the _PlacementRefDirection_ is given.

The direction of the y-axis of the _IfcGridPlacement_is the orthogonal complement to the x-axis. <font color="#0000ff">The
plane defined by the x and y axis shall be co-planar to the xy plane of
the local placement of the <i>IfcGrid</i>.</font>&nbsp;

> <small>NOTE
&nbsp;The <i>PlacementLocation.OffsetDistances[3]</i>
and the <i>PlacementRefDirection.OffsetDistances[3]</i>
shall either not be assigned or should have the same z offset value.</small>
>

The direction of the z-axis is the orientation of the cross product of the x-axis and the y-axis, <font color="#0000ff">i.e. the z-axis of the <i>IfcGridPlacement</i>
shall be co-linear to the z-axis of the local placement of the <i>IfcGrid</i>.</font>

> <font color="#0000ff" size="-1">HISTORY
&nbsp;New entity in IFC Release 1.5. The entity name was changed
from
IfcConstrainedPlacement. in IFC Release 2x.</font>
> 


****Geometry use definitions**:**

The following example shows the usage of placement location and direction for an _IfcGridPlacement_.

<table cellpadding="2" cellspacing="2"> <tbody>
<tr> <td align="left" valign="top"><a href="drawings/IfcGridPlacement-Layout1.dwf"><img src="figures/ifcgridplacement-layout1.gif" alt="without ref direction" border="0" height="300" width="400"></a></td> <td align="left" valign="top"><i>PlacementRefDirection</i>
is <u>not</u> given - the object coordinate system is
defined by: <ul> <li><u>its location</u>:
given by the virtual
grid intersection of <i>PlacementLocation</i></li> <li><u>its
x-axis direction</u>: given by the
tangent of the first intersecting axis in the offset location of the
virtual grid intersection</li> </ul> </td> </tr>
<tr> <td align="left" valign="top"><a href="drawings/IfcGridPlacement-Layout2.dwf"><img src="figures/ifcgridplacement-layout2.gif" alt="with ref direction" border="0" height="300" width="400"></a></td> <td align="left" valign="top"><i>PlacementRefDirection</i>
is given - the object coordinate system is defined by: <ul> <li><u>its
location</u>: given by the virtual
grid intersection of <i>PlacementLocation</i></li> <li><u>its
x-axis direction</u>: given by the
tangent of the line between the virtual grid intersection of the <i>PlacementLocation</i>
and the virtual grid intersection of the <i>PlacementRefDirection</i>.</li>
</ul> </td> </tr> </tbody>
</table>