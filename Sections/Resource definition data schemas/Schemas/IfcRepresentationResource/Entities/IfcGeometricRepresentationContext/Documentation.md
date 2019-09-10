**Definition from ISO/CD 10303-42:1992**: A geometric representation context is a representation context in which the geometric representation items are geometrically founded. A geometric representation context is a distinct coordinate space, spatially unrelated to other coordinate spaces.

**Definition
from IAI**: The _IfcGeometricRepresentationContext_ defines the context that applies to several shape representations of products within a project. It defines the type of the context in which the shape representation is defined, and the numeric precision applicable to the geometric representation items defined in this context. In addition it can be used to offset the project coordinate system from a global point of origin, using the _WorldCoordinateSystem_ attribute. The _TrueNorth_ attribute can be given, if the y axis of the _WorldCoordinateSystem_ does not point to the global northing.

> <font size="-1">NOTE
&nbsp;The inherited attribute <i>ContextType</i>
shall have one of the following recognized values: <strike>'Sketch',
'Outline', 'Design', 'Detail',</strike> <font color="#ff0000">'Model',
'Plan'</font>,
'NotDefined'.</font>
> 


The use of one instance of _IfcGeometricRepresentationContext_
to represent the model (3D) view is mandatory, the use of a second
instance of _IfcGeometricRepresentationContext_
to represent the plan (2D) view is optional (but needs to be given, if
there are scale dependent plan views), the additional scale or view
dependent contexts need to be handled by using the subtype _IfcGeometricRepresentationSubContext_
pointing to the model view (or the plan view) as the _ParentContext_.
> <font color="#0000ff"><small>NOTE
&nbsp;The definition
of this class relates to the STEP entity
geometric_representation_context. Please refer to ISO/IS 10303-42:1994
for the final definition of the formal standard.</small> </font>

> <small><font color="#0000ff">HISTORY
&nbsp;New Entity in IFC Release 2.0<br> <font color="#ff0000">IFC2x Edition 3 CHANGE &nbsp;Applicable
values for <i>ContextType</i>
are only 'Model',&nbsp; 'Plan', and&nbsp; 'NotDefined'. All
other sub contexts
are now handled by the new subtype in IFC2x Edition 2 <i>IfcGeometricRepresentationSubContext</i>.
Upward compatibility for file based exchange is guaranteed.</font></font>
</small>