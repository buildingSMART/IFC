**Definition from ISO 6707-1:1989**: Inclined way or floor joining two surfaces at different levels.

**Definition of IAI**: An vertical passageway which provides a human circulation link between one floor level and another floor level at a different elevation. It may include a landing as an intermediate floor slab. A ramp normally does not include steps (stepped ramps are out of scope for this IFC Release).

The ramp is a container entity that aggregates all components of the ramp, it represents. The aggregation is handled via the _IfcRelAggregates_ relationship, relating an _IfcRamp_ with the related flights (_IfcRampFlight_) and landings (_IfcSlab_ with type 'Landing').

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC
		Release 2.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcRamp_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcRamp_ are part of this IFC release:

* [Pset_RampCommon](../../psd/IfcSharedBldgElements/Pset_RampCommon.xml){ target="SOURCE"}: common property set for all ramp occurrences

****Geometry Use Definitions****:

The geometric representation of _IfcRamp_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Independent geometric representations should only be used when the _IfcRamp_ is not defined as an aggregate. If defined as an aggregate, the geometric representation is the sum of the representation of the components within the aggregate.

**Local placement**

The local placement for _IfcRamp_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

If the _LocalPlacement_ is given for the _IfcRamp_, then all components, which are aggregated to the ramp should use this placement as their relative placement.

**_Geometric Representations_**

If the _IfcRamp_ has components (referenced by _SELF\IfcProduct.IsDecomposedBy_) then no independent geometric representation shall be defined for the <font size="-1">IfcRamp</font>. The _IfcRamp_ is then geometrically represented by the geometric representation of its components. The components are accessed via _SELF\IfcProduct.IsDecomposedBy[1].RelatedObjects_.

If the _IfcRamp_ has no components defined (empty set of _SELF\IfcProduct.IsDecomposedBy_) then the _IfcRamp_ may be represented by an _IfcShapeRepresentation_ with the RepresentationType = 'Brep'.

**Illustration**:

<table cellpadding="2" cellspacing="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcRamp-Layout1.dwf"><img src="figures/ifcramp-layout1.gif" alt="ramp" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcRamp</i> defining only the local
			 placement for all components.</td> 
		</tr> 
	 </table>