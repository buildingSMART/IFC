**Definition from ISO 6707-1:1989**: Construction comprising a succession of horizontal stages (steps or landings) that make it possible to pass on foot to other levels.

A vertical passageway allowing occupants to walk (step) from one floor level to another floor level at a different elevation. It may include a landing as an intermediate floor slab.

The stair is a container entity that aggregates all components of the stair, it represents. The aggregation is handled via the _IfcRelAggregates_ relationship, relating an _IfcStair_ with the related flights (_IfcStairFlight_) and landings (_IfcSlab_ with type 'Landing').

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcStair_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcStair_ are part of this IFC release:

* [Pset_StairCommon](../../psd/IfcSharedBldgElements/Pset_StairCommon.xml){ target="SOURCE"}: common property set for all stair occurrences

****Geometry Use Definitions****:

The geometric representation of _IfcStair_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Independent geometric representations should only be used when the IfcStair is not defined as an aggregate. If defined as an aggregate, the geometric representation is the sum of the representation of the components within the aggregate.

**Local placement**

The local placement for _IfcStair_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

If the _LocalPlacement_ is given for the _IfcStair_, then all components, which are aggregated to the stair should use this placement as their relative placement.

**_Geometric Representation_**

If the _IfcStair_ has components (referenced by _SELF\IfcObject.IsDecomposedBy_) then no independent geometric representation shall defined for the _IfcStair_. The _IfcStair_ is then geometrically represented by the geometric representation of its components. The components are accessed via _SELF\IfcObject.IsDecomposedBy[1].RelatedObjects_.

If the _IfcStair_ has no components defined (empty set of _SELF\IfcObject.IsDecomposedBy_) then the _IfcStair_ may be represented by an _IfcShapeRepresentation_ with the RepresentationType = 'Brep'.

**Illustration**:

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcStair-Layout1.dwf"><img src="figures/ifcstair-layout1.gif" alt="stair" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcStair</i> defining only the local
			 placement for all components.</td> 
		</tr> 
	 </table>
