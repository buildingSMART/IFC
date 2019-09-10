**Definition from ISO 6707-1:1989**: Construction enclosing the building from above.

The _IfcRoof_ is a description of the total roof. It acts as a container entity, that aggregates all components of the roof, it represents. The aggregation is handled via the _IfcRelAggregates_ relationship, relating a roof (_IfcRoof_) with the related roof entities, like slabs (_IfcSlab_), rafters and purlins (_IfcBeam_), or other (included) roofs, such as dormers (_IfcRoof_).

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcRoof_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcRoof_ are part of this IFC release:

* [Pset_RoofCommon](../../psd/IfcSharedBldgElements/Pset_RoofCommon.xml){ target="SOURCE"}: common property set for all roof occurrences

****Quantity Use Definition****:

The quantities relating to the _IfcRoof_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. It is accessible by the inverse _IsDefinedBy_ relationship. The following quantities are foreseen, but will be subjected to the local standard of measurement:

<table cellpadding="2" cellspacing="2" border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i><b>Name</b></i></font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1"><i><b>Description</b></i></font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i><b>Value
			 Type</b></i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">TotalSurfaceArea</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total
			 (exposed to the outside) area of all roof slabs belonging to the roof. The
			 exact definition and calculation rules depend on the method of measurement
			 used.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityArea</i></font></td> 
		</tr> 
	 </table>

****Geometry Use Definitions****:

The geometric representation of _IfcRoof_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Independent geometric representations should only be used when the _IfcRoof_ is not defined as an aggregate. If defined as an aggregate, the geometric representation is the sum of the representation of the components within the aggregate.

**Local Position**

The local placement for _IfcRoof_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level..
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

If the _LocalPlacement_ is given for the _IfcRoof_, then all components, which are aggregated to the roof should use this placement as their relative placement.

**_Geometric Representation_**

If the _IfcRoof_ has components (referenced by_SELF\IfcObject.IsDecomposedBy_) then no independent geometric representation shall defined for the _IfcRoof_. The _IfcRoof_ is then geometrically represented by the geometric representation of its components. The components are accessed via _SELF\IfcObject.IsDecomposedBy[1].RelatedObjects_.

If the _IfcRoof_ has no components defined (empty set of _SELF\IfcObject.IsDecomposedBy_) then the _IfcRoof_ may be represented by an _IfcShapeRepresentation_ with the _RepresentationType_ = 'Brep'.

**Illustration**:

<table cellpadding="2" cellspacing="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcRoof-Layout1.dwf"><img src="figures/ifcroof-layout1.gif" alt="roof" width="399" height="274" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcRoof</i> defining only the local
			 placement for all components.</td> 
		</tr> 
	 </table>
