This enumeration defines the different types of spaces or space boundaries in terms of either being inside the building or outside the building.

**Enumeration**:

<table cellspacing="2" cellpadding="2">
      <tr>
        <td valign="top" align="left">
          INTERNAL
        </td>
        <td valign="top" align="left">
          <i>IfcSpace</i>
        </td>
        <td valign="top" align="left">
          The space is an internal space, fully enclosed by
          physical boundaries (directly or indirectly through
          adjacent spaces).
        </td>
      </tr>
      <tr>
        <td valign="top" align="left">
           
        </td>
        <td valign="top" align="left">
          <i>IfcSpaceBoundary</i>
        </td>
        <td valign="top" align="left">
          The space boundary faces to the inside of an internal
          space.
        </td>
      </tr>
      <tr>
        <td valign="top" align="left">
          EXTERNAL
        </td>
        <td valign="top" align="left">
          <i>IfcSpace</i>
        </td>
        <td valign="top" align="left">
          The space is an external space, not (or only partially)
          enclosed by physical boundaries.
        </td>
      </tr>
      <tr>
        <td valign="top" align="left">
           
        </td>
        <td valign="top" align="left">
          <i>IfcSpaceBoundary</i>
        </td>
        <td valign="top" align="left">
          The space boundary faces to the outer space, or the
          inside of an external space.
        </td>
      </tr>
      <tr>
        <td valign="top" align="left">
          NOTDEFINED
        </td>
        <td valign="top" align="left">
           
        </td>
        <td valign="top" align="left">
          No information available.
        </td>
      </tr>
    </table>

> <small><font color="#0000FF">HISTORY: New enumeration in
      IFC Release 2.0</font></small>