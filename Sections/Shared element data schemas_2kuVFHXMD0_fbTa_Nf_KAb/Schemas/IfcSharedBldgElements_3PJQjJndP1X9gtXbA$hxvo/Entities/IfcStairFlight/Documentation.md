Assembly of building components in a single "run" of stair steps (not interrupted by a landing). The stair steps and any stringers are included in this object. A winder is regarded as part of a stair flight.

An _IfcStairFlight_ is normally aggregated by a stair (_IfcStair_) through the _IfcRelAggregates_ relationship, the stair flight is then included in the set of _IfcRelAggregates.RelatedObjects_.

An _IfcStairFlight_ normally connects the floor slab of zero to two different storeys (or partial storeys) within a building. The connection relationship between the _IfcStairFlight_ and the _IfcSlab_ is expressed using the _IfcRelConnectsElements_ relationship.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0.</font>

****Property Set Use Definition****:

The property sets relating to the _IfcStairFlight_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcStairFlight_ are part of this IFC release:

* [Pset_StairFlightCommon](../../psd/IfcSharedBldgElements/Pset_StairFlightCommon.xml){ target="SOURCE"}: common property set for all stair flight occurrences

****Geometry Use Definitions****:

The geometric representation of _IfcStairFlight_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local placement**

The local placement for _IfcStairFlight_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level.
* If the _IfcStairFlight_, however, is used by an _IfcStair_, and this container class defines its own local placement, then the _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the aggregate.

**Standard Geometric Representation**

The standard geometric representation of _IfcStair_ is defined using the following multiple shape representations for its definition:

* **WalkingLine**: A two-dimensional open curve (_IfcBoundedCurve_) defining the walking line for the stair flight.
* **Boundary**: A two-dimensional closed curve (_IfcBoundedCurve_) defining the boundary of the stair flight.
* **Body**: A Brep representation (subtypes of _IfcManifoldSolidBrep_) defining the 3D shape of the stair flight

_First Representation: WalkingLine_

The walking line is represented by a two-dimensional open curve within a particular shape representation. The curve is directed (direction has to be interpreted as specified at the subtypes of IfcCurve).

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcStairFlight_01-Layout1.dwf"><img src="figures/IfcStairFlight_01-Layout1.gif" alt="walking line" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcShapeRepresentation</i><br><i>RepresentationIdentifier</i> :
			 'WalkingLine'<br><i>RepresentationType</i> : 'GeometricSet' 
			 <ul> 
				<li>In case of straight flights the curve set shall consists of a
				  single item of type <i>IfcPolyline</i>.</li> 
				<li>In case of winding flights the curve set shall consists of a
				  single item of type <i>IfcCompositeCurve</i>.</li> 
				<li>In case of a curved flight or a spiral flight the curve set
				  shall consists of a single item of type <i>IfcTrimmedCurve</i>.</li> 
			 </ul></td> 
		</tr> 
	 </table>

_Second Representation: Boundary_

The flight boundary is represented by a two-dimensional closed curve within a particular shape representation.

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><a href="drawings/IfcStairFlight_02-Layout1.dwf"><img src="figures/IfcStairFlight_02-Layout1.gif" alt="boundary" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcShapeRepresentation</i><br><i>RepresentationIdentifier</i> :
			 'Boundary'<br><i>RepresentationType</i> : 'GeometricSet' 
			 <ul> 
				<li>In case of straight flights the curve set shall consists of a
				  single item of type <i>IfcPolyline</i>.</li> 
				<li>In case of winding flights or curved flights the curve set
				  shall consists of a single item of type <i>IfcCompositeCurve</i>.</li> 
				<li>In case of a spiral flight the curve set shall consists of a
				  single item of type <i>IfcConic</i> or <i>IfcPolyline</i>.</li> 
			 </ul></td> 
		</tr> 
	 </table>

_Third Representation: Body_

The three dimensional shape of the flight is represented by a Brep representation.

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td valign="TOP" align="LEFT"><a href="drawings/IfcStairFlight_03-Layout1.dwf"><img src="figures/IfcStairFlight_03-Layout1.gif" alt="3D" width="393" height="299" border="0"></a></td> 
		  <td valign="TOP" align="LEFT"><i>IfcShapeRepresentation</i><br><i>RepresentationIdentifier</i> :
			 'Body'<br><i>RepresentationType</i> : 'Brep' </td> 
		</tr> 
	 </table>