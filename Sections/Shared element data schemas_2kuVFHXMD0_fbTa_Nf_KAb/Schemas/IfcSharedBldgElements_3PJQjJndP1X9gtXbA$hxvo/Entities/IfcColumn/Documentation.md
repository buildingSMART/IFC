**Definition from ISO 6707-1:1989**: Structural member of slender form, usually vertical, that transmits to its base the forces, primarily in compression, that are applied to it.

An _IfcColumn_ is a vertical structural member which often is aligned with a structural grid intersection. It represents a vertical, or nearly vertical, structural member from an architectural point of view. It is not required to be load bearing.

> <small>NOTE
&nbsp;For any longitudial structural member, not constrained to
be predominately horizontal nor vertical, or where this semantic
information is irrelevant, the entity <i>IfcMember</i>
exists.</small>
> 


> <font color="#0000ff" size="-1">HISTORY New entity in IFC Release 1.0 </font>

****Type Use Definition****

_IfcColumn_ defines the occuurence of any column, common information about beam types (or styles) is handled by _IfcColumnType_. The _IfcColumnType_ (if present) may establish the common&nbsp;type name, usage (or predefined) type, common material layer set, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcColumnType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

If no <span style="font-style: italic;">IfcColumnType</span> is attached&nbsp;(i.e. if only occurrence information is given) the predefined type may be given by using the _ObjectType_ attribute.&nbsp;Recommended values are 'column' (the default).

****Property Set Use Definition****:

The property sets relating to the _IfcColumn_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcColumn_ are part of this IFC release:

* [Pset_ColumnCommon](../../psd/IfcSharedBldgElements/Pset_ColumnCommon.xml){ target="SOURCE"}: common property set for all column occurrences

****Material
Use Definition****

The material of the _Ifc__Column_ is defined by the _IfcMaterial_ or _IfcMaterialList_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Material information can also be given at the _Ifc__Column__Type_, defining the common attribute data for all occurrences of the same type.&nbsp;It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _Ifc__Column__Type_._HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_ to _IfcMaterial_ or _IfcMaterialList_. If both are given, then the material directly assigned to _Ifc__Column_ overrides the material assigned to _Ifc__Column__Type_.

****Quantity Use Definition****:

The quantities relating to the _IfcColumn_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. It is accessible by the inverse _IsDefinedBy_ relationship. The following quantities are foreseen, but will be subjected to the local standard of measurement used:

<table border="1" cellpadding="2" cellspacing="2"> <tbody> <tr valign="top"> <td align="left" valign="top"><font size="-1"><i><b>Name</b></i></font></td>
<td align="left" valign="top" width="60%"><font size="-1"><i><b>Description</b></i></font></td>
<td align="left" valign="top"><font size="-1"><i><b>Value
Type</b></i></font></td> </tr> <tr>
<td align="left" valign="top"><font size="-1">NominalLength</font></td>
<td align="left" valign="top" width="60%"><font size="-1">Total nominal length of the column, not taking
into account any cut-out's or other processing features.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">CrossSectionArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the cross section (or profile) of
the column. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">OuterSurfaceArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the extruded surfaces of the column
(not taking into account the end cap areas), normally generated as
perimeter * length.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">TotalSurfaceArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the column, normally generated as
perimeter * length + 2 * cross section area.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total gross volume of the column, not taking into
account possible processing features (cut-out's, etc.) or openings and
recesses. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total net volume of the column, taking into
account possible processing features (cut-out's, etc.) or openings and
recesses. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total gross weight of the column without add-on
parts, not taking into account possible processing features (cut-out's,
etc.) or openings and recesses.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total net weight of the column without add-on
parts, taking into account possible processing features (cut-out's,
etc.) or openings and recesses.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> </tbody>
</table>

****Containment Use Definition****

The _IfcColumn_, as any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second (optional) relationship is the aggregation within an&nbsp;element assembly.

* The _IfcColumn_, is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The _IfcColumn_, may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype. In this case it should not be additionally contained in the project spatial hierarchy, i.e.&nbsp;_SELF\IfcElement.ContainedInStructure_should be _NIL._

****Geometry Use Definitions****:

The geometric representation of _IfcColumn_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local
Placement**

The local placement for _IfcColumn_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric
Representations_**

Currently, the use of 'SweptSolid', 'Clipping', and 'MappedRepresentation' representations is supported. In addition the general representation types 'SurfaceModel', 'Brep' and 'BoundingBox' are allowed. The geometry use definition for 'BoundingBox', 'SurfaceModel' and 'Brep' is explained at _IfcBuildingElement_.

**Swept
Solid Representation**

The standard geometric representation of _IfcColumn_ is defined using the 'SweptSolid' representation. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid**: _IfcExtrudedAreaSolid_ shall be supported 
* **Profile**: _IfcRectangleProfileDef_, _IfcCircleProfileDef_, _IfcEllipseProfileDef_, and&nbsp;_IfcArbitraryClosedProfileDef_ (including the subtype _IfcArbitraryProfileDefWithVoids_) shall be supported, in addition the support of basic steel profiles, such as _IfcIShapeProfileDef_, _IfcLShapeProfileDef_, _IfcUShapeProfileDef_, _IfcCShapeProfileDef_, _IfcZShapeProfileDef_, and _IfcTShapeProfileDef_ can be agreed. 
* **Extrusion**:&nbsp;All extrusion directions shall be supported

> EXAMPLE for standard geometric representation.

<table cellpadding="2" cellspacing="2"> <tbody> <tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcColumn_Standard-Layout1.dwf"><img src="figures/IfcColumn_Standard-Layout1.gif" alt="standard column" border="0" height="290" width="399"></a></td> <td align="left" valign="top"><small> </small> <blockquote><small>
</small> <p><small>The following interpretation of
dimension parameter applies for rectangular columns: </small></p>
<small> </small> <ul> <small> </small><li><small><i>IfcRectangleProfileDef.YDim</i>
interpreted as column width</small></li> <small> </small><li><small><i>IfcRectangleProfileDef.XDim</i>
interpreted as column height.</small></li> <small> </small>
</ul> <small> </small> <blockquote><small>
</small> <p><small>The following interpretation of
dimension parameter applies for round columns:</small></p> <small>
</small></blockquote> <small> </small> <ul>
<small> </small><li><small><i>IfcCircleProfileDef.Radius</i>
interpreted as column radius</small></li> <small> </small>
</ul> <small> </small></blockquote> </td>
</tr> <tr> <td><a href="drawings/IfcColumn_Advanced-Layout1.dwf"><img src="figures/IfcColumn_Advanced-Layout1.gif" alt="advanced column" border="0" height="290" width="399"></a></td> <td align="left" valign="top"> <blockquote><font size="-1">Use
of a special profile type (here <i>IfcIShapeProfileDef</i>)
for the definition of the <i>IfcExtrudedAreaSolid</i>.</font></blockquote>
</td> </tr> </tbody>
</table>

**Advanced SweptSolid and Clipping
Representation**

The advanced geometric representation of _IfcColumn_ is defined using the 'SweptSolid' (enhanced by additional profile types) or 'Clipping' geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid', or 'Clipping'

The following constraints apply to the advanced representation:

* **Solid**: see 'SwptSolid' geometric representation 
* **Profile**: see 'SwptSolid' geometric representation 
* **Extrusion**: see 'SwptSolid' geometric representation 
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_. 

> EXAMPLE for advanced geometric representation.

<table cellpadding="2" cellspacing="2"> <tbody>
<tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcColumn_Advanced-Layout1.dwf"><br> </a></td>
<td align="left" valign="top"><br> </td>
</tr> </tbody>
</table>

**MappedRepresentation**

In addition to the standard and advanced geometric representation of _IfcColumn_ that is defined using the 'SweptSolid' or 'Clipping' geometry, also the 'MappedRepresentation' shall be supported as it allows for reusing the geometry definition of the column type at all occurrences of the same type. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'MappedRepresentation'

The same constraints, as given for the&nbsp; 'SweptSolid' and&nbsp;'Clipping' geometric representation, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.