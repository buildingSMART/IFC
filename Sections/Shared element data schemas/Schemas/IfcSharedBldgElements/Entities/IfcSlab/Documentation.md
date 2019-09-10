A slab is a component of the construction that normally encloses a space vertically. The slab may provide the lower support (floor) or upper construction (roof slab) in any space in a building. It shall be noted, that only the core or constructional part of this construction is considered to be a slab. The upper finish (flooring, roofing) and the lower finish (ceiling, suspended ceiling) are considered to be coverings. A special type of slab is the landing, described as a floor section to which one or more stair flights or ramp flights connect. May or may not be adjacent to a building storey floor.

A slab may have openings, such as floor openings, or recesses. They are defined by an _IfcOpeningElement_ attached to the slab using the inverse relationship _HasOpenings_ pointing to _IfcRelVoidsElement_.

A particular usage type for the _IfcSlab_ can be given (if type information is available) by referring to the type object _IfcSlabType_, using the _IfcRelDefinesByType_ relationship, or (if only occurrence information is given) by using the _PredefinedType_ attribute. Values of the enumeration are 'Floor' (the default), 'Roof', 'Landing', 'Baseslab', 'Notdefined'. If the value 'UserDefined' is chosen, the user defined value needs to be given at the attribute _ObjectType_.&nbsp;

> <font color="#0000ff" size="-1">HISTORY: New entity in IFC
Release 2.0, it is a merger of the two previous entities IfcFloor,
IfcRoofSlab, introduced in IFC Release 1.0 </font>

****Type Use Definition****

The _IfcSlab_ defines the occuurence of any slab, common information about slab types (or styles) is handled by _IfcSlabType_. The _IfcSlabType_ (if present) may establish the common&nbsp;type name, usage (or predefined) type, common set of properties, common material layer set, and common shape representations (using _IfcRepresentationMap_). The _IfcSlabType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

As an additional use agreement for standard slabs (i.e. slabs with constant thickness along the extrusion direction), the _IfcSlabType_ should have a unique _IfcMaterialLayerSet_, that is referenced by the&nbsp;_IfcMaterialLayerSetUsage_ assigned to all occurrences of this slab type.

<table border="0" cellpadding="2" cellspacing="2" width="100%"><tbody><tr><td><p><img alt="Material layer set and usage" src="figures/ifcslab_materialusage-01.png" height="220" width="501">&nbsp;</p></td><td align="left" valign="top"><p><small>Assignment
of <i>IfcMaterialLayerSetUsage</i> and <i>IfcMaterialLayerSet</i>
to the slab type and the slab occurrence.</small></p></td></tr></tbody></table>

****Property Set Use Definition****:

The property sets relating to the _IfcSlab_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcSlab_ are part of this IFC release:

* [Pset_SlabCommon](../../psd/IfcSharedBldgElements/Pset_SlabCommon.xml){ target="SOURCE"}: common property set for all slab occurrences

****Material
Use Definition****

The material of the _IfcSlab_ is defined by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. For prismatic slabs, where the main face of the slab is extruded along the slab thickness, the material shall be defined by&nbsp;_IfcMaterialLayerSetUsage_. Multi-layer slabs can be represented by referring to several _IfcMaterialLayer_'s within the _IfcMaterialLayerSet_.&nbsp;

Material information can also be given at the _IfcSlabType_, defining the common attribute data for all occurrences of the same type.&nbsp;It is then accessible by the inverse _IsDefinedBy_ relationship pointing to_IfcSlabType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_. See Type Use Definition for additional agreements for standard slabs.

****Quantity Use Definition****

The quantities relating to the _IfcSlab_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table border="1" cellpadding="2" cellspacing="2"> <tbody> <tr valign="top">
<td align="left" valign="top"><font size="-1"><i><b>Name</b></i></font></td>
<td align="left" valign="top" width="60%"><font size="-1"><i><b>Description</b></i></font></td>
<td align="left" valign="top"><font size="-1"><i><b>Value
Type</b></i></font></td> </tr> <tr>
<td valign="top"><font size="-1">NominalWidth</font></td>
<td valign="top"><font size="-1">Total
nominal (or average) width (or thickness) of the slab. The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">Perimeter</font></td> <td align="left" valign="top" width="60%"><font size="-1">Perimeter measured along the outer boundaries of
the slab. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityLength</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossArea</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total area of the extruded area of
the slab. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td valign="top"><font size="-1">NetArea</font></td> <td valign="top"><font size="-1">Total area of the
extruded area of the slab, taking into account possible
slab openings. The exact definition and calculation rules depend on the
method of measurement used.</font></td> <td valign="top"><font size="-1"><i>IfcQuantityArea</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total gross volume of the slab, not taking into
account possible openings and recesses. The exact definition and
calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetVolume</font></td> <td align="left" valign="top" width="60%"><font size="-1">Total net volume of the slab, taking into account
possible openings and recesses. The exact definition and calculation
rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityVolume</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">GrossWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total gross weight of the slab, not taking into
account possible openings and recesses or projections. The exact
definition and calculation rules depend on the method of measurement
used.</font></td> <td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> <tr> <td align="left" valign="top"><font size="-1">NetWeight</font></td> <td align="left" valign="top" width="60%"><font size="-1"> Total net weight of the slab, taking into account
possible openings and recesses or projections. The exact definition and
calculation rules depend on the method of measurement used.</font></td>
<td align="left" valign="top"><font size="-1"><i>IfcQuantityWeight</i></font></td>
</tr> </tbody></table>

****Containment
Use Definition****

The _IfcSlab_, as any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second (optional) relationship is the aggregation within an&nbsp;element assembly.

* The&nbsp;_IfcSlab_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The&nbsp;_IfcSlab__may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype.    In this case it should not be additionally contained in the project spatial hierarchy, i.e.&nbsp;_SELF\IfcElement.ContainedInStructure_should be _NIL._

The _IfcSlab__&nbsp;_may also be an aggregate i.e. being composed by other elements and acting as an assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.IsDecomposedBy_. Components of a slab are described by instances of subtypes of _IfcBuildingElement_, with _IfcBuildingElementPart_ as a special focus subtype that are aggregated to form a complex slab. In this case, the contained elements should not be additionally contained in the project spatial hierarchy, i.e. the inverse attribute _SELF\IfcElement.ContainedInStructure_of _IfcBuildingElementPart_ (or other subtypes of _IfcBuildingElement_) should be _NIL._

****Geometry Use Definitions****The geometric representation of _IfcSlab_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

> <font size="-1">NOTE. If the <i>IfcSlab</i>
is of type Landing and is used within an <i>IfcStair</i>
or <i>IfcRamp</i>, the special agreements to handle stair
and ramp geometry will also affect the geometric representation of the <i>IfcSlab</i>.</font>
> 


**Local Placement**

The local placement for _IfcSlab_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the placement of the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the _IfcSlab_ is of type Landing and is used by an _IfcStair_ or _IfcRamp_, and this container class defines its own local placement, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the aggregate.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric
Representations_**

Currently, the use of 'SweptSolid', 'Clipping', 'Brep' and 'MappedRepresentation' representations is supported. In addition the general representation type 'BoundingBox' is allowed. The geometry use definitions for 'BoundingBox', and 'Brep' are explained at _IfcBuildingElement_.

**SweptSolid Representation**

The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used for the 'SweptSolid' representation:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the swept solid representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcArbitraryClosedProfileDef, IfcRectangleProfileDef, IfcCircleProfileDef, IfcEllipseProfileDef_ shall be supported. 
* **Extrusion**: The profile can be extruded perpendicularly or non-perpendicularly to the plane of the swept profile. ~~The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the _Position_ of the _IfcExtrudedAreaSolid_~~.

> EXAMPLE for standard geometric representation.

<table cellpadding="2" cellspacing="2"> <tbody> <tr valign="top">
<td align="left" valign="top"><a href="drawings/IfcSlab_Standard-Layout1.dwf"><img src="figures/ifcslab_standard-layout1.gif" alt="standard slab" border="0" height="274" width="399"></a></td><td align="left" valign="top"> <blockquote> <p>NOTE
The following interpretation of dimension parameter applies for
polygonal slabs (in ground floor view): </p> <ul> <li><i>IfcArbitraryClosedProfileDef
.OuterCurve</i>: closed bounded curve interpreted as area (or
foot print) of the slab. </li> </ul> </blockquote>
</td> </tr> </tbody></table>

**Clipping
representation**

The advanced geometric representation of _IfcSlab_ is defined using the swept area geometry with additional clippings applied. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'Clipping'

The following constraints apply to the advanced representation:

* **Solid**: see 'SweptSolid' shape representation, 
* **Profile**:&nbsp;see 'SweptSolid' shape representation, 
* **Extrusion**:&nbsp;see 'SweptSolid' shape representation, 
* **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_. 

> EXAMPLE for advanced geometric representation.

<table cellpadding="2" cellspacing="2"> <tbody><tr valign="top"> <td align="left" valign="top"><a href="drawings/IfcSlab_Advanced-Layout1.dwf"><img src="figures/ifcslab_advanced-layout1.gif" alt="advanced slab" border="0" height="274" width="399"></a></td>
<td align="left" valign="top">Definition of a roof
slab using advanced geometric representation. The profile is extruded
non-perpendicular and the slab body is clipped at the eave.</td> </tr>
</tbody></table>
