**Definition from ISO
6707-1:1989**: Vertical construction usually in masonry or in concrete which bounds or subdivides a construction works and fulfills a load bearing or retaining function.

The wall represents a vertical construction that bounds or subdivides spaces. Wall are usually vertical, or nearly vertical, planar elements, often designed to bear structural loads. A wall is however&nbsp;not required to be load bearing. The IFC specification provides two entities for wall occurrences:

* _IfcWallStandardCase_ &nbsp;used for all occurrences of walls, that have a non-changing thickness along the wall path and where the thickness parameter can be fully described by a material layer set. These walls are always represented geometrically by a SweptSolid geometry, if a 3D geometric representation is assigned.
* _IfcWall_ &nbsp;used for all other occurrences of wall, particularly for walls with changing thickness along the wall path (e.g. polygonal walls), or walls with a non-rectangular cross sections (e.g. L-shaped retaining walls), and walls having an extrusion axis that is unequal to the global Z axis of the project (i.e. non-vertical walls). 

> <font color="#0000ff" size="-1">HISTORY
New entity in IFC Release 1.0, the entity has changed in IFC Release 2x.</font>

****Type Use Definition****

_IfcWall_ (or the subtype _IfcWallStandardCase_) defines the occuurence of any wall, common information about&nbsp;wall types (or styles) is handled by _IfcWallType_. The _IfcWallType_ (if present) may establish the common&nbsp;type name, usage (or predefined) type, common material layer set, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcWallType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

****Property Set Use Definition****:

The property sets relating to the _IfcWall_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcWall_ are part of this IFC release:

* [Pset_WallCommon](../../psd/IfcSharedBldgElements/Pset_WallCommon.xml){ target="SOURCE"}: common property set for all wall occurrences

****Quantity Use Definition****:

The quantities relating to the _IfcWall_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table border="1" cellpadding="2" cellspacing="2"><tbody>
<tr valign="top"> <td align="left" valign="top"><font size="-1"><i><b>Name</b></i></font></td>
<td align="left" valign="top" width="60%"><font size="-1"><i><b>Description</b></i></font></td>
<td align="left" valign="top"><font size="-1"><i><b>Value
Type</b></i></font></td> </tr> <tr>
<td align="left" valign="top"><font size="-1">NominalLength</font></td>
<td align="left" valign="top" width="60%"><font size="-1">Total nominal (or average) length of the wall
along the wall path. The exact definition and calculation rules depend
on the method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td valign="top"><font size="-1">NominalWidth</font></td> <td valign="top"><font size="-1">Total
nominal (or average) width (or thickness) of the wall perpendicular to
the wall path. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td valign="top"><font size="-1">NominalHeight</font></td> <td valign="top"><font size="-1">Total
nominal (or average) height of the wall along the wall path. The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossFootprintArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by a ground floor view,
not taking any wall modifications (like recesses) into account. It is
also referred to as the foot print of the wall. The exact definition
and calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetFootprintArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by a ground floor view,
taking all wall modifications (like recesses) into account. It is also
referred to as the foot print of the wall. The exact definition and
calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossSideArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the middle plane of the wall.&nbsp; It does
not take into account any wall modifications (such as openings). The
exact definition and calculation rules depend on the method of
measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetSideArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the middle plane. It does
take into account all wall modifications (such as openings). The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr><tr> <td align="left" valign="top"><font size="-1">GrossSideAreaLeft</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the left side (when viewed along the wall path orientation). It does
not take into account any wall modifications (such as openings). The
exact definition and calculation rules depend on the method of
measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetSideAreaLeft</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the left side (when viewed along the wall path orientation). It does
take into account all wall modifications (such as openings). The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr><tr> <td align="left" valign="top"><font size="-1">GrossSideAreaRight</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the right side (when viewed along the wall path orientation). It does
not take into account any wall modifications (such as openings). The
exact definition and calculation rules depend on the method of
measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetSideAreaRight</font></td> <td align="left" valign="top" width="60%"><font size="-1">Area of the wall as viewed by an elevation view of
the right side (when viewed along the wall path orientation). It does
take into account all wall modifications (such as openings). The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Volume of the wall, without taking into account
the openings and the connection geometry. The exact definition and
calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Volume of the wall, after subtracting the openings
and after considering the connection geometry. The exact definition and
calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> </tbody></table>

****Containment
Use Definition****

The _IfcWall_ (and the subtype _IfcWallStandardCase_) as any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierarchical spatial containment, the second (optional) relationship is the aggregation within an&nbsp;element assembly.

* The _IfcWall_is places within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The&nbsp;_IfcWall__may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype.    In this case the wall should not be additionally contained in the project spatial hierarchy, i.e.&nbsp;_SELF\IfcElement.ContainedInStructure_should be _NIL._

The&nbsp;_IfcWall&nbsp;_may also be an aggregate i.e. being composed by other elements and acting as an assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.IsDecomposedBy_. Components of a wall are described by instances of _IfcBuildingElementPart_ that are aggregated to form a complex wall.   
In this case, the contained&nbsp;_IfcBuildingElementPart_'s should not be additionally contained in the project spatial hierarchy, i.e. the inverse attribute _SELF\IfcElement.ContainedInStructure_of _IfcBuildingElementPart_should be _NIL._

****Geometry Use Definitions****:
The geometric representation of _IfcWall_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The local placement for _IfcWall_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Currently, the use of 'SweptSolid', 'Clipping', and 'Brep' representations is supported. In addition the general representation types 'SurfaceModel' and 'BoundingBox' are allowed. The geometry use definition for 'BoundingBox', 'SurfaceModel' and 'Brep' is explained at _IfcBuildingElement_. A more restricted geometry definition is given at the level of the subtype _IfcWallStandardCase_.

**SweptSolid representation**

The standard geometric representation (for body) of _IfcWall_ is defined using the 'SweptSolid' representation. <font color="#0000ff">If
the wall body can be described by a
vertical extrusion of a polygonal footprint of the wall body (where
vertical = into the direction of the global Z axis), the subtype <i>IfcWallStandardCase
</i>should be used</font>. If the extrusion is not equal to global Z, then the _IfcWall_ with 'SweptSolid representation should be used. The _IfcShapeRepresentation_ shall have the following values:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef_ shall be supported. 
* **Extrusion**:&nbsp;The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the Position of the _IfcExtrudedAreaSolid_.

****Connection Geometry****

The connection between two walls is represented by the _IfcRelConnectsPathElements_. The use of the parameter of that relationship object is defined at the level of the subtypes of _IfcWall_ and at the _IfcRelConnectsPathElements_.
