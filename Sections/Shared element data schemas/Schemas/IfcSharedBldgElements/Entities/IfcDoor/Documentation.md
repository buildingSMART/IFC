**Definition from ISO 6707-1:1989**: Construction for closing an opening, intended primarily for access with hinged, pivoted or sliding operation.

The door is a building element that is predominately used to provide controlled access for people and goods. It includes constructions with hinged, pivoted, sliding, and additionally revolving and folding operations. A door consists of a lining and one or several panels, properties concerning the lining and panel are defined by the _IfcDoorLiningProperties_ and the _IfcDoorPanelProperties_.

The door entity, _IfcDoor_, defines a particular occurrence of a door inserted in the spatial context of a project. A door can:

* either be inserted as a filler in an opening, then the _IfcDoor_ has an inverse attribute _FillsVoids_ provided,
* or be a "free standing" door, then the _IfcDoor_ has no&nbsp;inverse attribute _FillsVoids_ provided.

The actual parameter of the door and/or its shape are defined by the _IfcDoor_ as the occurrence definition (or project instance), or by&nbsp;the _IfcDoorStyle_ as the specific definition (or project type). Parameters are given:

* at the _IfcDoor_ for occurrence specific parameters. The _IfcDoor_ specifies:
    * the door width and height
    * the door opening direction (by the y-axis of the _ObjectPlacement_)

* at the _IfcDoorStyle_, to which the _IfcDoor_ is related by the inverse relationship _IsDefinedBy_ pointing to _IfcRelDefinesByType_, for style parameters common to all occurrences of the same style.
    * the operation type (single swing, double swing, revolving, etc.)
    * the door hinge side (by using two different styles for right and left opening doors)
    * the construction type
    * the particular attributes for the lining by the _IfcDoorLiningProperties_
    * the particular attributes for the panels by the&nbsp;_IfcDoorPanelProperties_


The _IfcDoor_ is normally inserted into an _IfcOpeningElement_ (but does not need to - see above) using the _IfcRelFillsElement_ relationship. It is also directly linked to the spatial structure of the project (and here normally to the _IfcBuildingStorey_, or to the _IfcSpace_) using the _IfcRelContainedInSpatialStructure_ relationship.

> <font color="#0000ff" size="-1">HISTORY
New entity in IFC
Release 1.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcDoor_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcDoor_ are part of this IFC release:

* [Pset_DoorCommon](../../psd/IfcSharedBldgElements/Pset_DoorCommon.xml){ target="SOURCE"}: common property set for all door occurrences
* [Pset_DoorWindowGlazingType](../../psd/IfcSharedBldgElements/Pset_DoorWindowGlazingType.xml){ target="SOURCE"}: specific property set for the glazing properties of the door glazing, if available
* [Pset_DoorWindowShadingType](../../psd/IfcSharedBldgElements/Pset_DoorWindowShadingType.xml){ target="SOURCE"}: specific property set for the shading properties of the door glazing, if available

****Geometry Use Definitions****:

The geometric representation of _IfcDoor_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. The _IfcDoor_, in case of an occurrence object, gets its parameter and shape from the _IfcDoorStyle_. If an _IfcRepresentationMap_ (a block definition) is defined for the _IfcDoorStyle_, then the _IfcDoor_ inserts it through the _IfcMappedItem_.

**Local Placement**

The local placement for _IfcDoor_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

1. The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the same element (if given), in which the _IfcDoor_ is used as a filling (normally an _IfcOpeningElement_), as provided by the _IfcRelFillsElement_ relationship.
2. If the _IfcDoor_ is not inserted into an _IfcOpeningElement_, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
3. If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**_Geometric Representation_**

The&nbsp;geometric representation of _IfcDoor_ is defined using the following (potentially&nbsp;multiple) _IfcShapeRepresentation_'s for its _IfcProductDefinitionShape_:

* **Profile**: A&nbsp;'GeometricCurveSet' consisting of a single closed curve defining the outer boundary of the door (lining). The door parametric representation uses this profile in order to apply the door lining and panel parameter. If not provided, the profile of the _IfcOpeningElement_ is taken.
* **FootPrint**: A 'GeometricCurveSet', or 'Annotation2D' representation defining the 2D shape of the door
* **Body**: A 'SweptSolid', 'SurfaceModel', or 'Brep' representation defining the 3D shape of the door.

In addition the parametric representation of a (limited) door shape is available by applying the parameters from _IfcDoorStyle_ referencing _IfcDoorLiningProperties_ and _IfcDoorPanelProperties_. The purpose of the parameter is described at those entities and below (door opening operation by door style).

**Profile -&nbsp;'GeometricCurveSet' representation**

The door profile is represented by a three-dimensional closed curve within a particular shape representation. The profile is used to apply the parameter of the parametric door representation.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Profile'
* _RepresentationType_ : 'GeometricCurveSet', only a single closed curve shall be contained in the set of _IfcShapeRepresentation.Items_.

A 'Profile' representation has to be provided if:

* a parametric representation shall be applied to the door AND
    * the&nbsp;door is 'free standing', or
    * the opening into which the&nbsp;door is inserted is not extruded horizontally (i.e. where the opening profile does not match the&nbsp;door profile)


**FootPrint -&nbsp;'GeometricCurveSet'
or 'Annotation2D' representation**

The door foot print is represented by a set of two-dimensional&nbsp;curves (or in case of 'Annotation2D' additional hatching and text) within a particular shape representation. The foot print is used for the planview representation of the door.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'FootPrint'
* _RepresentationType_ : 'GeometricCurveSet', or 'Annotation2D'

**Body - 'SweptSolid', 'SurfaceModel', or
'Brep' representation**

The door body is either represented parameterically (see parametric representation) or by explicit 3D shape. The 3D shape is given by using extrusion geometry, or surface models, or Brep models within a particular shape representation. The body is used for the model view representation of the door.&nbsp;The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid', 'SurfaceModel', or 'Brep'

**MappedRepresentation**

The 'FootPrint' and 'Body' geometric representation of _IfcDoor_ can be shared among several identical doors using the 'MappedRepresentation'. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'FootPrint', 'Body'
* _RepresentationType_ : 'MappedRepresentation'

The same constraints, as given for the&nbsp; 'FootPrint', 'Body' representation identifiers, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.

****Door opening operation by door style****

The parameters that defines the shape of the _IfcDoor_, are given at the _IfcDoorStyle_ and the property sets, which are included in the _IfcDoorStyle_. The _IfcDoor_ only defines the local placement which determines the opening direction of the door. <font color="#0000ff">The overall size of
the <i>IfcDoor</i> to be used to apply the lining or panel
parameter provided by the <i>IfcDoorStyle</i> is
determined by the IfcShapeRepresentation with the
RepresentationIdentifier = 'Profile'. Only in case of an <i>IfcDoor</i>
inserted into an <i>IfcOpeningElement</i> using the <i>IfcRelFillsElement</i>
relationship, having a horizontal extrusion (along the y-axis of the <i>IfcDoor</i>),
the overall size is determined by the extrusion profile of the <i>IfcOpeningElement</i>.</font>

> <small>Note
&nbsp;The&nbsp;<i>OverallWidth</i> and <i>OverallHeight</i>
parameters are for informational purpose only.</small>
>

<small></small><table border="1" cellpadding="2" cellspacing="2">
<tbody> <tr valign="top"> <td align="left" valign="top"><small><img alt="fig 1" src="figures/ifcdoor-fig01.gif" height="130" width="150"><br>
</small></td> <td align="left" valign="top"><small>The
door panel (for swinging
doors) opens always into the direction of the positive Y axis of the
local placement. The determination of whether the door opens to the
left or to the right is done at the level of the <i>IfcDoorStyle</i>.
Here it is a left side opening door given by&nbsp;<i>IfcDoorStyle.OperationType</i>
= SingleSwingLeft</small></td> </tr> <tr> <td><small><img alt="fig 2" src="figures/ifcdoor-fig02.gif" height="130" width="150"><br> </small></td> <td valign="top"><small>If the door should open to
the other side, then the local placement has to be changed. It is still
a left side opening door, given by <i>IfcDoorStyle.OperationType</i>
= SingleSwingLeft</small></td> </tr> <tr> <td><img alt="fig 3" src="figures/ifcdoor-fig03.gif" height="130" width="150"></td> <td valign="top"><small>If the door panel (for swinging
doors) opens to the right, a separate door style needs to be used (here
<i>IfcDoorStyle.OperationType</i>
= SingleSwingRight) and it always
opens into the direction of the positive Y axis of the
local placement.&nbsp;</small></td> </tr> <tr valign="top"> <td align="left" valign="top"><small><img alt="fig 4" src="figures/ifcdoor-fig04.gif" height="130" width="150"><br> </small></td> <td align="left" valign="top"><small>If the
door panel (for swinging doors) opens to the right, and into the
opposite directions, the local placement of the door need
to change. The door style is given by <i>IfcDoorStyle.OperationType</i>
= SingleSwingRight.</small></td> </tr> </tbody>
</table>
