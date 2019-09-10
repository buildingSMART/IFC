An _IfcMember_ is a structural member designed to carry loads between or beyond points of support. It is not required to be load bearing. The location of the member (being horizontal, vertical or sloped) is not relevant to its definition (in contrary to _IfcBeam_ and _IfcColumn_).

> <small> </small><small><font color="#0000ff">HISTORY
New entity in IFC Release 2x2 Addendum. </font> <br> <font color="#ff0000">IFC2x2
ADDENDUM CHANGE The entity <i>IfcMember</i> has been
added. Upward compatibility for file based exchange is guaranteed.</font></small>
> 


****Type Use Definition****

_IfcMember_ defines the occuurence of any member, common information about member types (or styles) is handled by _IfcMemberType_. The _IfcMemberType_ (if present) may establish the common&nbsp;type name, usage (or predefined) type, common material layer set, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcMemberType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

If no <span style="font-style: italic;">IfcMemberType</span> is attached&nbsp;(i.e. if only occurrence information is given) the predefined type may be given by using the _ObjectType_ attribute.&nbsp;Recommended values are 'member' (the default), 'brace', 'collar', 'member', 'post', 'purlin', 'rafter', 'stringer', 'strut'.

****Property Set Use Definition****

The property sets relating to the _IfcMember_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcMember_ are part of this IFC release:

* [Pset_MemberCommon](../../psd/IfcSharedBldgElements/Pset_MemberCommon.xml){ target="SOURCE"}: common property set for all member occurrences

****Material Use Definition****

The material of the _IfcMember_is defined by the _IfcMaterial_ or _IfcMaterialList_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Material information can also be given at the&nbsp;_IfcMember___Type_, defining the common attribute data for all occurrences of the same type.&nbsp;It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _IfcMember__Type_._HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_ to _IfcMaterial_ or _IfcMaterialList_. If both are given, then the material directly assigned to _IfcMember_overrides the material assigned to&nbsp;_IfcMember___Type_.

****Quantity Use Definition****

The quantities relating to the _IfcMember_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following quantities are foreseen, but will be subjected to the local standard of measurement used:

<table border="1" cellpadding="2" cellspacing="2">
<tbody> <tr valign="top"> <td align="left" valign="top"><font size="-1"><i><b>Name</b></i></font></td>
<td align="left" valign="top" width="60%"><font size="-1"><i><b>Description</b></i></font></td>
<td align="left" valign="top"><font size="-1"><i><b>Value
Type</b></i></font></td> </tr> <tr>
<td align="left" valign="top"><font size="-1">NominalLength</font></td>
<td align="left" valign="top" width="60%"><font size="-1">Total nominal length of the member, not taking
into account any cut-out's or other processing features.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">CrossSectionArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the cross section (or profile) of
the member. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">OuterSurfaceArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the extruded surfaces of the member
(not taking into account the end cap areas), normally generated as
perimeter * length.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">TotalSurfaceArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the member, normally generated as
perimeter * length + 2 * cross section area.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total gross volume of the member, not taking into
account possible processing features (cut-out's, etc.) or openings and
recesses. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total net volume of the member, taking into
account possible processing features (cut-out's, etc.) or openings and
recesses. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total gross weight of the member without add-on
parts, not taking into account possible processing features (cut-out's,
etc.) or openings and recesses.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total net weight of the member without add-on
parts, taking into account possible processing features (cut-out's,
etc.) or openings and recesses.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> </tbody>
</table>

****Containment Use Definition****

The _IfcMember_, as any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second (optional) relationship is the aggregation within an&nbsp;element assembly.

* The _IfcMember_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The _IfcMember_ may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype. 

****Geometry Use Definition****

The geometric representation of _IfcMember_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The local placement for _IfcMember_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**_Geometric Representations_**

Currently, the use of 'SweptSolid', 'Clipping', and 'MappedRepresentation' representations is supported. In addition the general representation types 'SurfaceModel', 'Brep', and 'BoundingBox' are allowed. The geometry use definition for 'BoundingBox', 'SurfaceModel' and 'Brep' is explained at _IfcBuildingElement_.

**SweptSolid Representation**

The standard geometric representation of _IfcMember_ is defined using the 'SweptSolid' representation. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ shall be supported 
* **Profile**: All subtypes of _IfcParameterizedProfileDef_ and _IfcArbitraryClosedProfileDef_ (including the subtype _IfcArbitraryProfileDefWithVoids_) shall be supported (exclusions need to be agreed upon by implementer agreements).
* **Extrusion**: All extrusion directions shall be supported.

> <font size="-1"><u>EXAMPLE</u>:
standard geometric representation. </font>

<table cellpadding="2" cellspacing="2"> <tbody>
<tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcBeam_Standard-Layout1.dwf"><img src="figures/ifcbeam_standard-layout1.gif" alt="standard beam" border="0" height="299" width="393"></a></td>
<td align="left" valign="top"> <blockquote> <p><font size="-1">The following
interpretation of dimension parameter applies for rectangular members: </font></p>
<ul> <li><font size="-1"><i>IfcRectangleProfileDef.YDim</i>
interpreted as member width</font></li> <li><font size="-1"><i>IfcRectangleProfileDef.XDim</i>
interpreted as member depth</font></li> </ul> </blockquote>
<blockquote><font size="-1">The following
interpretation of dimension parameter applies for circular members: </font>
<ul> <li><font size="-1"><i>
IfcCircleProfileDef</i> Radius interpreted as member radius.</font></li>
</ul> </blockquote> </td> </tr> <tr> <td><a href="drawings/IfcBeam_Advanced-1-Layout1.dwf"><img src="figures/ifcbeam_advanced-1-layout1.gif" alt="non-perpendicular extrusion" border="0" height="299" width="393"></a></td> <td align="left" valign="top"> <blockquote> <p><font size="-1">Use of <i>IfcBooleanClippingResult</i>
between an <i>IfcExtrudedAreaSolid</i> and an <i>IfcHalfSpaceSolid</i>
to create a clipped body.</font></p> </blockquote> </td>
</tr> </tbody>
</table>

**Clipping Representation**

The advanced geometric representation of _IfcBeam_ is defined using the 'Clipping' geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'Clipping'

The following constraints apply to the advanced representation:

* **Solid**: see 'SweptSolid' geometric representation 
* **Profile**: see 'SweptSolid' geometric representation 
* **Extrusion**:&nbsp;see 'SweptSolid' geometric representation
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or its subtypes). 

> <font size="-1"><u>EXAMPLE</u>
advanced geometric representation </font>

<table cellpadding="2" cellspacing="2"> <tbody>
<tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcBeam_Advanced-2-Layout1.dwf"><img src="figures/ifcbeam_advanced-2-layout1.gif" alt="clipped beam" border="0" height="299" width="393"></a></td>
<td align="left" valign="top"> <blockquote><font size="-1">Use of <i>IfcBooleanClippingResult</i>
between an <i>IfcExtrudedAreaSolid</i> and an <i>IfcHalfSpaceSolid</i>
to create a clipped body.</font></blockquote> </td> </tr>
</tbody>
</table>

**MappedRepresentation**

In addition to the &nbsp;'SweptSolid' and the 'Clipping' geometric representation of _IfcMember_&nbsp;also the 'MappedRepresentation' shall be supported as it allows for reusing the geometry definition of the member type at all occurrences of the same type. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'MappedRepresentation'

The same constraints, as given for the&nbsp;'SweptSolid' and the 'Clipping' geometric representation, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.
