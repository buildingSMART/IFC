﻿The window is a building element that is predominately used to provide natural light and fresh air. It includes vertical opening but also horizontal opening such as skylights or light domes. It includes constructions with swinging, pivoting, sliding, or revolving panels and fixed panels. A window consists of a lining and one or several panels.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1  
> Construction for closing a vertical or near vertical opening in a wall or pitched roof that will admit light and may admit fresh air.

The _IfcWindow_ defines a particular occurrence of a window inserted in the spatial context of a project. A window can:

* be inserted into an _IfcOpeningElement_ using the _IfcRelFillsElement_ relationship, then the _IfcWindow_ has an inverse attribute _FillsVoids_ provided,
* be part of an element assembly, often an _IfcCurtainWall_, using the _IfcRelAggregates_ relationship, then the inverse attribute _Decomposes_ is provided.
* or be a "free standing" window, then the _IfcWindow_ has no inverse attributes _FillsVoids_ or _Decomposes_ provided.

> NOTE&nbsp; View definitions or implementer agreements may restrict the relationship to only include one window (or door) into one opening.

There are two entities for window occurrences:

* _IfcWindowStandardCase_ used for all occurrences of windows, that have a 'Profile' shape representation defined to which a set of shape parameters for lining and framing properties apply. Additionally it requires the provision of an _IfcWindowType_ that references one _IfcWindowLiningProperties_ and on to many _IfcWindowPanelProperties_. 
* _IfcWindow_ used for all other occurrences of windows, particularly for windows having only 'Brep', or 'SurfaceModel' geometry without applying shape parameters.

The actual parameter of the window and/or its shape is defined at the _IfcWindow_ as the occurrence definition (or project instance), or by the _IfcWindowType_ as the specific definition (or project type). The following parameters are given:

* at the _IfcWindow_ or _IfcWindowStandardCase_ for occurrence specific parameters. The _IfcWindow_ specifies:
*  
    * the window width and height
    * the window opening direction (by the y-axis of the _ObjectPlacement_) 
* at the _IfcWindowType_ to which the _IfcWindow_ is related by the inverse relationship _IsDefinedBy_ pointing to _IfcRelDefinesByType_, for type parameters common to all occurrences of the same type.
*  
    * the partitioning type (single panel, double panel, tripel panel, more panels)
    * the operation type (swing, tilt and turn, pivot revolve, fixed case ment, etc.)
    * the window panel hinge side (by using two different styles for right and left opening windows)
    * the construction material type
    * the particular attributes for the lining by the _IfcWindowLiningProperties_
    * the particular attributes for the panels by the  _IfcWindowPanelProperties_ 

> HISTORY&nbsp; New entity in IFC1.0.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The attributes _PredefinedType_ and _OperationType_ are added, the applicable type object has been changed to _IfcDoorType_.

{ .use-head}
Parameteric Representation using parameters at _IfcWindowType_

The parameters, which define the shape of the _IfcWindow_, are given at the _IfcWindowType_ and the property sets, which are included in the _IfcWindowType_. The _IfcWindow_ only defines the local placement. The overall size of the _IfcWindow_ to be used to apply the lining or panel parameter provided by the _IfcWindowType_ is determined by the IfcShapeRepresentation with the RepresentationIdentifier = 'Profile'. Only in case of an _IfcWindow_ inserted into an _IfcOpeningElement_ using the _IfcRelFillsElement_ relatioship, having a horizontal extrusion (along the y-axis of the _IfcDoor_), the overall size is determined by the extrusion profile of the _IfcOpeningElement_.

Figure 1 illustrates the insertion of a window into the _IfcOpeningElement_ by creating an instance of _IfcWindow_ with _PartitioningType = DoublePanelHorizontal_. The parameters _OverallHeight_ and _OverallWidth_ show the extent of the window in the positive Z and X axis of the local placement of the window. The lining and the transom are created by the given parameters.

!["window 1"](../../../../../../figures/ifcwindow-layout1.gif "Figure 1 &mdash; Window placement")

Figure 2 illustrates the final window (DoublePanelHorizontal) with first panel having _PanelPosition = TOP_, _OperationType = BOTTOMHUNG_ and second panel having _PanelPosition = BOTTOM_ and _OperationType = TILTANDTURNLEFTHAND_.

!["window 2"](../../../../../../figures/ifcwindow-layout2.gif "Figure 2 &mdash; Window planes")

{ .use-head}
Window opening operation by window type

The parameters that defines the shape of the _IfcWindow_, are given at the _IfcWindowType_ and the property sets, which are included in the _IfcWindowType_. The _IfcWindow_ only defines the local placement which determines the opening direction of the window. The overall layout of the _IfcWindow_ is determined by its _IfcWindowType.PartitioningType_. Each window panel has its own operation type, provided by _IfcWindowPanelProperties.OperationType_. All window panels are assumed to open into the same direction (if relevant for the particular window panel operation. The hindge side (whether a window opens to the left or to the right) is determined by the _IfcWindowPanelProperties_._OperationType_.

> NOTE&nbsp;  There are different conventions in different countries on how to show the symbolic presentation of the window panel operation (the "triangles"). Either as seen from the exterior, or from the interior side. The following figures show the symbolics from the exterior side (the convention as used predominately in Europe).

Figure 3 illustrates window operation types.

<table><tr><td><table border="1" cellpadding="2" cellspacing="2">
<tbody>
<tr valign="top">
<td align="left" valign="top"><small><img alt="fig 1" src="../../../../../../figures/ifcwindow-fig01.gif" height="121" width="301"><br></small></td>
<td align="left" valign="top">
<p><small>The window panel (for side hung windows) opens always
into the direction of the positive Y axis of the local placement.
The determination of whether the window opens to the left or to
the right is done at
<em>IfcWindowPanelProperties.OperationType</em>. Here it is a left
side opening window given by <em>OperationType</em> =
SideHungLeftHand.</small></p>
</td>
</tr>
<tr>
<td><small><img alt="fig 2" src="../../../../../../figures/ifcwindow-fig02.gif" height="121" width="301"><br></small></td>
<td valign="top">
<p><small>If the window should open to the other side, then the
local placement has to be changed. It is still a left hung
window, given by <em>IfcWindowPanelProperties.OperationType</em>
= SideHungLeftHand.</small></p>
</td>
</tr>
<tr>
<td><img alt="fig 3" src="../../../../../../figures/ifcwindow-fig03.gif" height="121" width="301"></td>
<td valign="top">
<p><small>If the window panel (for side hung windows) opens to
the right, a separate window panel style needs to be used (here
<em>IfcWindowPanelProperties.OperationType</em>
= SideHungRightHand) and it always opens into the direction of
the positive Y axis of the local placement. </small></p>
</td>
</tr>
<tr valign="top">
<td align="left" valign="top"><small><img alt="fig 4" src="../../../../../../figures/ifcwindow-fig04.gif" height="121" width="301"><br></small></td>
<td align="left" valign="top">
<p><small>If the window should open to the other side, then the
local placement has to be changed. It is still a right hung
window, given by <em>IfcWindowPanelProperties.OperationType</em>
= </small><small>SideHungRightHand.</small></p>
<small>.</small></td>
</tr>
</tbody>
</table>

</td></tr>
<tr><td><p class="figure">Figure 3 &mdash; Window operations</p></td></tr>
</table>
