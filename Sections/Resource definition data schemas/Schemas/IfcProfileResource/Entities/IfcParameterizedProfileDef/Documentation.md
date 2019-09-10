The parameterized profile definition defines a 2D position coordinate system to which the parameters of the different profiles relate to. All profiles are defined centric to the origin of the position coordinate system, or more specific, the origin [0.,0.] shall be in the center of the bounding box ~~gravity~~ of the profile.

The _Position_ attribute of the _IfcParameterizedProfileDef_ is used to position the profile within the XY plane of the underlying coordinate system of the swept surface geometry, the swept area solid or the sectioned spine. It can be used to position the profile at any cardinal point that becomes the origin [0.,0.,0.] of the extruded or rotated surface or solid.

> <small> <font color="#0000ff">HISTORY&nbsp;
New entity in
Release IFC2x Edition 2.</font></small>

> <font color="#ff0000"><small>IFC2x
Platform CHANGE&nbsp; The <i>IfcParameterizedProfileDef</i>
is introduced as an intermediate new abstract entity that unifies the
definition and usage of the position coordinate system for all
parameterized profiles. The Position attribute has been removed at all
subtypes (like <i>IfcRectangleProfileDef</i>, <i>IfcCircleProfileDef</i>,
etc.).<br>
IFC2x Edition 3 CHANGE&nbsp; All profile
origins are now in the center of the bounding box.</small> </font>