Inclined slab segment, normally providing a human circulation link between two landings, floors or slabs at different elevations.

An _IfcRampFlight_ is normally aggregated by a ramp (_IfcRamp_) through the _IfcRelAggregates_ relationship, the ramp flight is then included in the set of _IfcRelAggregates.RelatedObjects_.

A ramp flight normally connects the floor slab of zero to two different storeys (or partial storeys) within a building. The connection relationship between the _IfcRampFlight_ and the _IfcSlab_ is expressed using the _IfcRelConnectsElements_ relationship.

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC
		Release 2.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcRampFlight_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcRampFlight_ are part of this IFC release:

* [Pset_RampFlightCommon](../../psd/IfcSharedBldgElements/Pset_RampFlightCommon.xml){ target="SOURCE"}: common property set for all ramp flight occurrences

****Geometry Use Definitions****:

The geometric representation of _IfcRampFlight_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local placement**

The local placement for _IfcRampFlight_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the _IfcRampFlight_, however, is used by an _IfcRamp_, and this container class defines its own local placement, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point to the local placement of the aggregate.

**Standard Geometric Representation**

The standard geometric representation of _IfcRampFlight_ is defined using the swept area geometry. The following constraints apply to the standard representation:

* **Solid**: _IfcExtrudedAreaSolid_ is required,
* **Profile**: _IfcRectangleProfileDef_ shall be supported. 
* **Extrusion**: The profile shall be extruded in any direction relative to the XY plane of the position coordinate system of the _IfcExtrudedAreaSolid_. Therefore non-perpendicular sweep operation has to be supported. It might be further constrained to be in the direction of the global z-axis in implementers agreements. 

<table cellpadding="2" cellspacing="2"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcRampFlight-Layout1.dwf"><img src="figures/IfcRampFlight-Layout1.gif" alt="fig1" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT">Example of geometric representation of
			 <i>IfcRampFlight</i>.</td> 
		</tr> 
	 </table>