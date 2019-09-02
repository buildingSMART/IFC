An _IfcPlate_ is a planar and often flat part with constant thickness. A plate can be a structural part carrying loads between or beyond points of support, however it is not required to be load bearing.&nbsp;The location of the plate (being horizontal, vertical or sloped) is not relevant to its definition (in contrary to _IfcWall_ and _IfcSlab_ (as floor slab)).&nbsp;

> <small>NOTE &nbsp;Plates are&nbsp;normally
made of steel, other metallic material, or by glass panels. However the
definition of <i>IfcPlate</i> is material independent and
specific material information shall be handled by using <i>IfcAssociatesMaterial</i>
to assign a material specification to the <i>IfcPlate</i>.&nbsp;</small>
> 
> <small>NOTE &nbsp;Although not necessarily, plates
are often add-on parts. This
is represented by
the <i>IfcRelAggregates</i> decomposition
mechanism used to aggregate parts, such as <i>IfcPlate</i>,
into a container element, e.g. <i>IfcElementAssembly</i>,
or <i>IfcCurtainWall</i>.&nbsp;</small>
> 


An instance _IfcPlate_ should preferably get its geometric representation and material assignment through the type definition by _IfcPlateType_ assigned using the _IfcRelDefinesByType_ relationship. This allows identical plates in a construction to be represented by the same instance of _IfcPlateType_.

> <font color="#0000ff"><small>
HISTORY New entity in IFC
Release 2x2 </small></font>

****Property Set Use Definition****:

The property sets relating to the _IfcPlate_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcPlate_ are part of this IFC release:

* [Pset_PlateCommon](../../psd/IfcSharedBldgElements/Pset_PlateCommon.xml){ target="SOURCE"}: common property set for all plate occurrences 

****Containment Use Definitions****

The _IfcPlate_, as any subtype of _IfcBuildingElement_, may participate in two different containment relationships. The first (and in most implementation scenarios mandatory) relationship is the hierachical spatial containment, the second relationship is the aggregation within an&nbsp;element assembly.

* The&nbsp;_IfcPlate_ is placed within the project spatial hierarchy using the objectified relationship _IfcRelContainedInSpatialStructure_, referring to it by its inverse attribute _SELF\IfcElement.ContainedInStructure_. Subtypes of&nbsp;_IfcSpatialStructureElement_ are valid spatial containers, with _IfcBuildingStorey_ being the default container.
* The&nbsp;_IfcPlate_ may be aggregated into an element assembly using the objectified relationship _IfcRelAggregates_, referring to it by its inverse attribute _SELF\IfcObjectDefinition.Decomposes_. Any subtype of _IfcElement_ can be an element assembly, with _IfcElementAssembly_ as a special focus subtype. In this case, no additional relationship to the spatial hierarchy shall be given (i.e.&nbsp;_SELF\IfcElement.ContainedInStructure_ = NIL), the relationship to the spatial container is handled by the element assembly.__ 

****Geometry use definition****The geometric representation of _Ifc__Plate_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**

The local placement for _Ifc__Plate_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that.
    * If the _IfcPlate_ is part of an assembly, the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the container element, e.g. _&nbsp;IfcElementAssembly_, 

* If the relative placement is not used, the absolute placement is defined within the world coordinate system.

**_Geometric Representations_**

Currently, the use of 'SweptSolid', 'Clipping', 'Brep' and 'MappedRepresentation' representations is supported. In addition the general representation types 'SurfaceModel' and 'BoundingBox' are allowed. The geometry use definition for 'BoundingBox', 'SurfaceModel' and 'Brep' is explained at _IfcBuildingElement_.

**SweptSolid Representation**  
The standard geometric representation of _IfcPlate_ is defined using the 'SweptSolid' representation. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

**Clipping Representation**  
The advanced geometric representation of _IfcMember_is defined using the 'Clipping' geometry. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'Clipping'

**MappedRepresentation**  
In addition to the standard geometric representation of _Ifc__Plate_ that is defined using the 'SweptSolid' or 'Clipping' geometry, also the 'MappedRepresentation' shall be supported as it allows for reusing the geometry definition of the member type at all occurrences of the same type. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'MappedRepresentation'

The same constraints, as given for the standard 'SweptSolid' and the advanced 'SweptSolid' and 'Clipping' geometric representation, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.

****Use definition for steel members****

When using the _IfcPlate_ for steel members in steel construction applications the following additional conventions apply:

**Definition by non-geometric properties**  
Additional non-geometric properties can be specified through the class _IfcPropertySet_, which is attached to the inverse attribute _IfcObject.IsDefinedBy_ through the objectified relationship _IfcRelDefinesByProperties_. This allows for attaching country-specific information to structural members.

**Decomposition**  
An instance of _IfcPlate_ can be part of a decomposition through the _IfcRelAggregates_ relationship - both as sub-ordinate or as a super-ordinate component.

* If the _IfcPlate_ instance is a sub-ordinate component (i.e. the plate is an add-on part), its local placement shall be relative to that of the super-ordinate instance. 
* As a super-ordinate component, the sub-ordinates of _IfcPlate_ can be other plates or instances of _IfcProxy_, or _IfcDiscreteAccessory_ (like _IfcFastener_). 

**Position number**  
The position number is assigned through the attribute _IfcElement.Tag_