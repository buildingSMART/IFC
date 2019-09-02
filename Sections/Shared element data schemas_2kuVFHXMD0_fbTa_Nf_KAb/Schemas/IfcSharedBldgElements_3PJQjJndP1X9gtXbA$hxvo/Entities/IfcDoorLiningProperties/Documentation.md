**Definition
of IAI**: The door lining is the frame which enables the door leaf to be fixed in position. The door lining is used to hang the door leaf. The parameters of the door lining (_IfcDoorLiningProperties_) define the geometrically relevant parameter of the lining.

The _IfcDoorLiningProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcDoorStyle_. More information about the door lining can be included in the same list of the _IfcDoorStyle_ using the _IfcPropertySet_ for dynamic extensions.

> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC Release 2.0</font>

****Geometry
Use Definitions****

The _IfcDoorLiningProperties_ does not hold its own geometric representation. However it defines parameters which can be used to create the shape of the door style (which is inserted by the _IfcDoor_ into the spatial context of the project).

**Interpretation
of parameter**

The parameters of the _IfcDoorLiningProperties_ define a standard door lining, including (if given) a threshold and a transom. The outer boundary of the lining is determined by the occurrence parameter assigned to the _IfcDoor_, which inserts the _IfcDoorStyle_.

<table border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorLiningProperties-Fig01.gif" alt="lining 1" border="0" height="155" width="247"></td>
      <td align="left" valign="top">The
lining is applied to the left, right and upper side of the opening
reveal. The parameters are:
      <ul>
        <li><i>LiningDepth</i>,
          <font color="#0000ff">if
omitted, equal to wall thickness - this only takes effect if a value for
          <i>LiningThickness</i>
is given. If both parameters are not given, then there is no lining.</font></li>
        <li><i>LiningThickness</i></li>
      </ul>
      </td>
    </tr>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorLiningProperties-Fig02.gif" alt="lining 2" border="0" height="129" width="210"> </td>
      <td align="left" valign="top">The
lining can only cover part of the opening reveal.
      <ul>
        <li><i>LiningOffset</i>
: given if lining edge has an offset to the x axis of the local
placement.</li>
      </ul>
      <blockquote><small>NOTE
&nbsp;In addition to the&nbsp;<i>LiningOffset</i>,
the local placement of the <i>IfcDoor</i>
can already have an offset to the wall edge and thereby shift the
lining along the y axis. The actual position of the lining is
calculated from the origin of the local placement along the positive y
axis with the distance given by <i>LiningOffset</i>.</small></blockquote>
      </td>
    </tr>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorLiningProperties-Fig03.gif" alt="lining 3" border="0" height="132" width="227"></td>
      <td align="left" valign="top">The
lining may include a casing, which covers part of the wall faces around
the opening. The casing covers the left, right and upper side of the
lining on both sides of the wall. The parameters are:
      <ul>
        <li><i>CasingDepth</i></li>
        <li><i>CasingThickness</i></li>
      </ul>
      </td>
    </tr>
    <tr>
      <td align="left" valign="top"><img src="figures/IfcDoorLiningProperties-Fig04.gif" alt="lining 4" border="0" height="206" width="181"></td>
      <td align="left" valign="top">The
lining may include a threshold, which covers the bottom side of the
opening. The parameters are:
      <ul>
        <li><i>ThresholdDepth<font color="#0000ff">, </font></i><font color="#0000ff">if omitted, equal to wall thickness -
this only takes effect if a value for <i>ThresholdThickness
          </i>is given. If both
parameters are not given, then there is no threshold.</font></li>
        <li><i>ThresholdThickness</i></li>
        <li><i>ThresholdOffset</i>
(not shown in figure): given, if the threshold edge has an offset to
the x axis of the local placement. </li>
      </ul>
      </td>
    </tr>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorLiningProperties-Fig05.gif" alt="lining 5" border="0" height="332" width="342"></td>
      <td align="left" valign="top">The
lining may have a transom which separates the door panel from a window
panel. The transom, if given, is defined by:
      <ul>
        <li><i>TransomOffset</i>
: a parallel edge to the x axis of the local placement</li>
        <li><i>TransomThickness</i></li>
      </ul>
      <p>The depth of the transom
is identical to the depth of the lining and not given as separate
parameter.</p>
      </td>
    </tr>
  </tbody>
</table>

> <font size="-1">NOTE: special agreement on <i>LiningDepth</i>
  <br>
It describes the length of the lining along the reveal of the door
opening. It can be given by an absolute value, if the door lining has a
specific depth depending on the door style. However often it is equal
to the wall thickness. If the same door style is used (like the same
type of single swing door), but inserted into different walls with
different thicknesses, it would be necessary to create a special door
style for each wall thickness. Therefore several CAD systems allow to
set the value to "automatically aligned" to wall thickness. This should
be exchanged by leaving the optional attribute LiningDepth unassigned.</font>
> 


> <font size="-1">NOTE: the same agreement applies to <i>ThresholdDepth</i></font>
>