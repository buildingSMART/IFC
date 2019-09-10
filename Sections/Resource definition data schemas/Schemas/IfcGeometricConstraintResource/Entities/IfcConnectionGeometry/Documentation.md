The _IfcConnectionGeometry_ is used to describe the geometric and topological constraints that facilitate the physical connection of two objects. It is envisioned as a control that applies to the element connection relationships.

> <small>
NOTE&nbsp; The element
connection relationship normally provides for a logical connection
information, by referencing the relating and related elements. If in
addition an <i>IfcConnectionGeometry</i> is provided,
physical connection information is given by specifying exactly where at
the relating and related element the element connection occurs. <font color="#0000ff">Using the eccentricity subtypes, the
connection can also be described when there is a physical distance (or
eccentricity) between the connection elements</font>.</small>

The _IfcConnectionGeometry_ allows for the provision of connection constraints between geometric and topological elements, the following connection geometry/topology types are in scope:

<ul>
  <li>point | <font color="#0000ff">vertex point</font>,
  </li>
  <li>curve | <font color="#0000ff">edge curve</font>,
  </li>
  <li>surface | <font color="#0000ff">face surface</font>,
  </li>
  <li>profile - <font color="#ff0000" size="-1">NOTE&nbsp;&nbsp;the
profile (or port) connection type is deprecated since Release IFC2x
Edition 2.</font></li>
</ul>
> <small>
  <font color="#0000ff">HISTORY&nbsp;
New entity in IFC Release 1.5.</font> <br>
  <font color="#ff0000">IFC2x Edition 3 CHANGE&nbsp;
The definition of the subtypes has been enhanced by allowing either
geometric representation items (point | curve | surface) or topological
representation items with associated geometry (vertex point | edge
curve | face &nbsp;surface).</font>
  </small>