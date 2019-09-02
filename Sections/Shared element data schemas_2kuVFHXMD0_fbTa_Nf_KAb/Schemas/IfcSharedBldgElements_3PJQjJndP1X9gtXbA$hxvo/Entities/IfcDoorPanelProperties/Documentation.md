A description of the door panel. A door panel is normally a door leaf that opens to allow people or goods to pass. The parameters of the door panel define the geometrically relevant parameter of the panel,

The _IfcDoorPanelProperties_ are included in the list of properties , given by attribute _HasPropertySets_ of the _IfcDoorStyle_. More information about the door panel can be included in the same list of the _IfcDoorStyle_ using the _IfcPropertySet_ for dynamic extensions.

> <small><font color="#0000ff">HISTORY&nbsp;
New Entity in IFC Release 2.0.</font></small>

****Geometry Use Definitions****

The _IfcDoorPanelProperties_ does not hold an own geometric representation. However it defines parameter, which can be used to create the shape of the door style (which is inserted by the _IfcDoor_ into the spatial context of the project).

**Interpretation of parameters**

The parameters of the _IfcDoorPanelProperties_ define a standard door panel, including (if given) a proportional width to define non-uniform double swing (or sliding, or folding) doors. The outer boundary of the panel is determined by the occurrence parameter assigned to the _IfcDoor_, which inserts the _IfcDoorStyle_. It has to take the lining parameter into account as well.

<table border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorPanelProperties-Fig01.gif" alt="panel 1" border="0" height="187" width="266"></td>
      <td align="left" valign="top">The depth of
the panel (swinging, double-acting, and sliding panels) is defined by
the <i>PanelDepth</i> parameter.
      <ul>
        <li><i>PanelDepth</i></li>
      </ul>
      </td>
    </tr>
    <tr valign="top">
      <td align="left" valign="top"><img src="figures/IfcDoorPanelProperties-Fig02.gif" alt="panel 2" border="0" height="259" width="304"></td>
      <td align="left" valign="top">For door
operation types that include more than one panel, the width of (at
least) one panel is given by a normalised ratio measure. It determines
the width of that panel, which is defined as a ratio of the overall
width of the door opening.
      <ul>
        <li><i>PanelWidth</i></li>
      </ul>
      </td>
    </tr>
  </tbody>
</table>