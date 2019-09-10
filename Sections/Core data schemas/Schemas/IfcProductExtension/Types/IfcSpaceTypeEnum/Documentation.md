This enumeration defines the available generic types for _IfcSpace_ and _IfcSpaceType_.

> HISTORY&nbsp; New enumeration in IFC2x3.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The enumerators INTERNAL and EXTERNAL have been added for upward compatibility to replace _InteriorOrExteriorSpace_ usage.

{ .spec-head}
Enumerated Item Definitions:

<ul>
<li><b>SPACE</b>: Any space not falling into another category.<br>
<ul style="list-style-type:none;">
<li><small>NOTE&nbsp; For classification of spaces according to its
function that is often determined by national classification
systems use <em>IfcClassificationReference</em> via the
relationship <em>IfcRelAssociatesClassification</em>.</small></li>
</ul>
</li>
<li><b>PARKING</b>: A space dedication for use as a parking spot
for vehicles, including access, such as a parking aisle</li>
<li><b>GFA</b>: Gross Floor Area - a specific kind of space for
each building story that includes all net area and construction
area (also the external envelop). Provision of such a specific
space is often required by regulations.</li>
<li><b>INTERNAL:</b>
<ul style="list-style-type:none;">
<li><small><font color="#FF0000">NOTE&nbsp; the use is deprecated and
only provided for backward compatibility
purposes.</font></small></li>
</ul>
</li>
<li><b>EXTERNAL</b>:<br>
<ul style="list-style-type:none;">
<li><small><font color="#FF0000">NOTE&nbsp; the use is deprecated and
only provided for backward compatibility
purposes.</font></small></li>
</ul>
</li>
</ul>
