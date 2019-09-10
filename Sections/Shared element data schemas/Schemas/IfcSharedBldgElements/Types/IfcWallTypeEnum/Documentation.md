This enumeration defines the different types of walls that can further specify an _IfcWall_ or _IfcWallType_.

> HISTORY&nbsp; New enumeration in IFC2x2.

{ .change-ifc2x2}
> IFC2x2 CHANGE&nbsp; The enumerator _POLYGON_ has been changed to _POLYGONAL_.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The enumerators _ELEMENTEDWALL_ and _PLUMBINGWALL_ have been added.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; New enumerators MOVABLE, PARAPET, PARTITIONING, and SOLIDWALL have been added.  
> IFC4 DEPRECATION&nbsp; The enumerators STANDARD, POLYGONAL and ELEMENTEDWALL are deprecated and shall no longer be used.

{ .spec-head}
Enumerated Item Definitions:

<ul>
<li><b>MOVABLE</b>: A movable wall that is either movable, such as
folding wall or a sliding wall, or can be easily removed as a
removable partitioning or mounting wall. Movable walls do normally
not define space boundaries and often belong to the furnishing
system.</li>
<li><b>PARAPET</b>: A wall-like barrier to protect human occupants
from falling, or to prevent the spread of fires. Often designed at
the edge of balconies, terraces or roofs.</li>
<li><b>PARTITIONING</b>: A wall designed to partition spaces that
often has a light-weight, sandwich-like construction (e.g. using
gypsum board). Partitioning walls are normally non load
bearing.</li>
<li><b>PLUMBINGWALL</b>: A pier, or enclosure, or encasement,
normally used to enclose plumbing in sanitary rooms. Such walls
often do not extent to the ceiling.</li>
<li><b>SHEAR</b>: A wall designed to withstand shear loads. Such
shear walls are often designed having a non-rectangular cross
section along the wall path. Also called retaining walls or
supporting walls they are used to protect against soil layers
behind.</li>
<li><b>SOLIDWALL</b>: A massive wall construction for the wall core
being the single layer or having multiple layers attached. Such
walls are often masonry or concrete walls (both cast in-situ or
precast) that are load bearing and fire protecting.</li>
<li><b>STANDARD</b>: A standard wall, extruded vertically with a
constant thickness along the wall path.
<blockquote class="deprecated">The value is deprecated, it is
expressed by choosing the subtype <em>IfcWallStandardCase</em><br>
&nbsp;</blockquote>
</li>
<li><b>POLYGONAL</b>: A polygonal wall, extruded vertically, where
the wall thickness varies along the wall path.
<blockquote class="deprecated">The value is deprecated, it is
expressed by choosing the type <em>IfcWall</em> with a footprint
geometry being polygonal.<br>
&nbsp;</blockquote>
</li>
<li><b>ELEMENTEDWALL</b>: A stud wall framed with studs and faced
with sheetings, sidings, wallboard, or plasterwork.
<blockquote class="deprecated">The value is deprecated, it is
expressed by choosing the subtype <em>IfcWallElementedCase</em><br>
&nbsp;</blockquote>
</li>
<li><b>USERDEFINED</b>: User-defined wall element.</li>
<li><b>NOTDEFINED</b>: Undefined wall element</li>
</ul>
> NOTE&nbsp; The potentially misleading term _SHEAR_ shall not impose a particular resistance against shear forces, but a particular shape.
