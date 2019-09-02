**Definition
form ISO 6707-1:1989**: Construction for closing a vertical or near vertical opening in a wall or pitched roof that will admit light and may admit fresh air.

**Definition from
IAI**: A window consists of a lining and one or several panels. Properties concerning the lining and panel(s) are defined by the _IfcWindowLiningProperties_ and the _IfcWindowPanelProperties_.

The window entity (_IfcWindow_) defines a particular occurrence of a window inserted in the spatial context of a project. The actual parameter of the window and/or its shape is defined at the _IfcWindowStyle_, to which the _IfcWindow_ is related by the inverse relationship _IsDefinedBy_ pointing to _IfcRelDefinesByType_. The _IfcWindowStyle_ also defines the particular attributes for the lining (_IfcWindowLiningProperties_) and panels (_IfcWindowPanelProperties_). Therefore:

* the _IfcWindow_ is the occurrence definition (or project instance)
* the _IfcWindowStyle_ is the specific definition (or project type)

The _IfcWindow_ is normally inserted into an _IfcOpeningElement_ (but does not need to) using the _IfcRelFillsElement_ relationship. It is also directly linked to the spatial structure of the project (and here normally to the _IfcBuildingStorey_) using the _IfcRelContainedInSpatialStructure_ relationship.

> <font color="#0000ff" size="-1">HISTORY New entity in IFC Release 1.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcWindow_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcWindow_ are part of this IFC release:

* [Pset_WindowCommon](../../psd/IfcSharedBldgElements/Pset_WindowCommon.xml){ target="SOURCE"}: common property set for all window occurrences
* [Pset_DoorWindowGlazingType](../../psd/IfcSharedBldgElements/Pset_DoorWindowGlazingType.xml){ target="SOURCE"}: specific property set for the glazing properties of the window glazing, if available
* [Pset_DoorWindowShadingType](../../psd/IfcSharedBldgElements/Pset_DoorWindowShadingType.xml){ target="SOURCE"}: specific property set for the shading properties of the window glazing, if available

****Geometry
Use Definitions****:

The geometric representation of _IfcWindow_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. The _IfcWindow_, in case of an occurrence object, gets its parameter and shape from the _IfcWindowStyle_. If an _IfcRepresentationMap_ (a block definition) is defined for the _IfcWindowStyle_, then the _IfcWindow_ inserts it through the _IfcMappedItem_ (referred to by _IfcShapeRepresentation.Items_).

**Local
Placement**

The local placement for _IfcWindow_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

1. The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the same element (if given), in which the _IfcWindow_ is used as a filling (normally an _IfcOpeningElement_), as provided by the _IfcRelFillsElement_ relationship.
2. If the _IfcWindow_ is not inserted into an _IfcOpeningElement_, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
3. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**_Geometric Representation_**

The&nbsp;geometric representation of _IfcWindow_ is defined using the following (potentially&nbsp;multiple) _IfcShapeRepresentation_'s for its _IfcProductDefinitionShape_:

* **Profile**: A&nbsp;'GeometricCurveSet' consisting of a single losed curve defining the outer boundary of the window (lining). The&nbsp;window parametric representation uses this profile in order to apply the&nbsp;window lining and panel parameter. If not provided, the profile of the _IfcOpeningElement_ is taken.
* **FootPrint**: A 'GeometricCurveSet', or 'Annotation2D' representation defining the 2D shape of the&nbsp;window
* **Body**: A 'SweptSolid', 'SurfaceModel', or 'Brep' representation defining the 3D shape of the&nbsp;window.

In addition the parametric representation of a (limited)&nbsp;window shape is available by applying the parameters from&nbsp;_IfcWindow__Style_ referencing&nbsp;_IfcWindow__LiningProperties_ and&nbsp;_IfcWindow__PanelProperties_. The purpose of the parameter is described at those entities and below (parametric representation).

**Profile -&nbsp;'GeometricCurveSet' representation**

The&nbsp;window profile is represented by a three-dimensional closed curve within a particular shape representation. The profile is used to apply the parameter of the parametric&nbsp;window representation.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Profile'
* _RepresentationType_ : 'GeometricCurveSet', only a single closed curve shall be contained in the set of _IfcShapeRepresentation.Items_.

A 'Profile' representation has to be provided if:

* a parametric representation shall be applied to the window&nbsp;AND
    * the window is 'free standing', or
    * the opening into which the window is inserted is not extruded horizontally (i.e. where the opening profile does not match the window profile)


**FootPrint -&nbsp;'GeometricCurveSet' or
'Annotation2D' representation**

The&nbsp;window foot print is represented by a set of two-dimensional&nbsp;curves (or in case of 'Annotation2D' additional hatching and text) within a particular shape representation. The foot print is used for the plan view representation of the&nbsp;window.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'FootPrint'
* _RepresentationType_ : 'GeometricCurveSet', or 'Annotation2D'

**Body - 'SweptSolid', 'SurfaceModel', or 'Brep'
representation**

The&nbsp;window body is either represented parameterically (see parametric representation) or by explicit 3D shape. The 3D shape is given by using extrusion geometry, or surface models, or Brep models within a particular shape representation. The body is used for the model view representation of the&nbsp;window.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid', 'SurfaceModel', or 'Brep'

**MappedRepresentation**

The 'FootPrint' and 'Body' geometric representation of&nbsp;_IfcWindow_ can be shared among several identical&nbsp;windows using the 'MappedRepresentation'. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'FootPrint', 'Body'
* _RepresentationType_ : 'MappedRepresentation'

The same constraints, as given for the&nbsp; 'FootPrint', 'Body' representation identifiers, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.

**Parameteric Representation using parameters given by _IfcWindowStyle_**

The parameters, which define the shape of the _IfcWindow_, are given at the _IfcWindowStyle_ and the property sets, which are included in the _IfcWindowStyle_. The _IfcWindow_ only defines the local placement. The overall size of the _IfcWindow_ is determined by its _OverallWidth_ and _OverallHeight_ parameter, if omitted, it should be taken from the profile of the _IfcOpening_, in which the _IfcWindow_ is inserted.

> EXAMPLE Inserting the _IfcWindowStyle.OperationType_ = DoublePanelHorizontal

<table border="1" cellpadding="2" cellspacing="2"> <tbody> <tr>
<td><a href="drawings/IfcWindow-Layout1.dwf"><img src="figures/IfcWindow-Layout1.gif" alt="window 1" border="0" height="299" width="356"></a></td>
<td align="left" valign="top">The insertion of the
window style into the IfcOpeningElement by creating an instance of
IfcWindow. The parameter: <ul><li><i>OverallHeigth</i></li><li><i>OverallWidth</i></li></ul>
<p>show the extend of the window in the positive Z and X axis of
the local placement of the window. The lining and the transom are
created by the given parameter (the flag <i>ParameterTakesPrecedence</i>
= TRUE).</p> <p>The representation type of the inserted
window is</p> <ul><li><i>IfcShapeRepresentation.RepresentationType</i>
= 'MappedRepresentation'</li></ul> </td> </tr>
<tr> <td><a href="drawings/IfcWindow-Layout2.dwf"><img src="figures/IfcWindow-Layout2.gif" alt="window 2" border="0" height="299" width="356"></a></td>
<td align="left" valign="top">The final window
(DoublePanelHorizontal) with <ul><li>first panel<br>
PanelPosition = TOP<br>
OperationType = BOTTOMHUNG</li><li>second panel<br>
PanelPosition = BOTTOM<br>
OperationType = TILTANDTURNLEFTHAND</li></ul> </td> </tr>
</tbody>
</table>

****Window
opening operation by window style****

The parameters that defines the shape of the _IfcWindow_, are given at the _IfcWindowStyle_ and the property sets, which are included in the _IfcWindowStyle_. The _IfcWindow_ only defines the local placement which determines the opening direction of the window. The overall layout of the _IfcWindow_ is determined by its&nbsp;_IfcWindowStyle.OperationType_. Each window panel has its own operation type, provided by _IfcWindowPanelProperties.OperationType_. All window panels are assumed to open into the same direction (if relevant for the particular window panel operation. The hinge side (whether a window opens to the left or to the right) is determined by the _Ifc__WindowPanelProperties_._OperationType_.

<table border="1" cellpadding="2" cellspacing="2"><tbody>
<tr valign="top"> <td align="left" valign="top"><small><img alt="fig 1" src="figures/IfcWindow-Fig01.gif" height="121" width="301"><br></small></td>
<td align="left" valign="top"><p><small>The
window panel (for side hung windows) opens always into the direction of
the positive Y axis of the
local placement. The determination of whether the window opens to the
left or to the right is done at <i>IfcWindowPanelProperties.OperationType</i>.
Here it is a left side opening window given by&nbsp;<i>OperationType</i>
= SideHungLeftHand.</small></p></td> </tr> <tr>
<td><small><img alt="fig 2" src="figures/IfcWindow-Fig02.gif" height="121" width="301"><br> </small></td> <td valign="top"><p><small>If
the window should open to
the other side, then the local placement has to be changed. It is still
a left hung window, given by <i>IfcWindowPanelProperties.OperationType</i>
=&nbsp;SideHungLeftHand.</small></p></td>
</tr> <tr> <td><img alt="fig 3" src="figures/IfcWindow-Fig03.gif" height="121" width="301"></td> <td valign="top"><p><small>If
the window panel (for side hung windows)
opens to the right, a separate window panel style needs to be used
(here <i>IfcWindowPanelProperties.OperationType</i>
=&nbsp;SideHungRightHand) and it always
opens into the direction of the positive Y axis of the
local placement.&nbsp;</small></p></td> </tr>
<tr valign="top"> <td align="left" valign="top"><small><img alt="fig 4" src="figures/IfcWindow-Fig04.gif" height="121" width="301"><br> </small></td><td align="left" valign="top"><p><small>If
the window should open to
the other side, then the local placement has to be changed. It is still
a right hung window, given by <i>IfcWindowPanelProperties.OperationType</i>
=&nbsp;</small><small>SideHungRightHand.</small></p><small>.</small></td>
</tr> </tbody></table>