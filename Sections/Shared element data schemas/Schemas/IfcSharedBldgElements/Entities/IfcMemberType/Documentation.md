The element type (_IfcMemberType_) defines a list of commonly shared property set definitions of a structural member and an optional set of product representations. It is used to define a structural member specification (i.e. the specific product information that is common to all occurrences of that product type).

> <font size="-1">NOTE: The product representations are defined as
		  representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		  gets assigned by an element occurrence instance through the
		  <i>IfcShapeRepresentation.Item[1]</i> being an
		  <i>IfcMappedItem</i>.</font>
>

A structural member type is used to define the common properties of a certain type of a structural member that may be applied to many instances of that type to assign a specific style. Structural member types may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcMemberType_ are represented by instances of _IfcMember_.

> <font color="#0000FF" size="-1">HISTORY New entity in Release IFC2x
		  Edition 2.</font>
>

> <font color="#FF0000" size="-1">IFC2x2 ADDENDUM CHANGE: The
		entity <i>IfcMember</i> has been added to serve as the occurrence object for
		all member types.</font>

**Use definition for steel members**

When using the _IfcMemberType_ as the underlying type for steel members within steel construction aware applications the following additional conventions apply:

**Material association:******  
The _IfcMemberType_ is associated with exactly one instance _IfcMaterial_ by the _IfcRelAssociatesMaterial_ relationship. This material association assigns a common material to all occurrences (_IfcBeam_, _IfcColumn_ or _IfcBuildingElementProxy_) of the _IfcMemberType_. If an individual occurrence has its own material assignment (see _IfcMember_), then this overrides the material assignment given at the _IfcMemberType_.

**Geometric representation:******  
The _IfcMemberType_ type has (at least) one representation map assigned through the _RepresentationMaps_ relation. The representation map has a full geometric representation given by:

*  _IfcExtrudedAreaSolid_ for straight beams,
* _IfcRevolvedAreaSolid_ for curved beams based on circular arcs, or 
* _IfcSurfaceCurveSweptAreaSolid_ for all other curved beams. 

The attribute _ProfileName_ of the extruded _IfcProfile_ instance may contain a standardized name according to local standards. However, a geometric representation of the profile is necessary as specified below. An importing application is allowed to check for the existence of the profile name: in case of identifying it as a standardized name, the corresponding profile geometry and possibly other cross sectional properties can be read from a library. Otherwise the explicit IFC geometry and possible non geometric _IfcProfileProperties_ have to be used.

Only 'SweptSolid' representation should be used to represent steel members. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Body'
* _RepresentationType_ : 'SweptSolid'

The following additional constraints apply to the 'SweptSolid' representation:

* **Solid:** _IfcExtrudedAreaSolid_ shall be supported.
* **Profile:** _IfcArbitraryClosedProfileDef, IfcArbitraryOpenProfileDef, IfcArbitraryProfileDefWithVoids, IfcCircleProfileDef, IfcCompositeProfileDef, IfcIShapeProfileDef, IfcRectangleProfileDef, IfcRoundedRectangleProfileDef, IfcCShapeProfileDef, IfcCircleHollowProfileDef, IfcCraneRailAShapeProfileDef, IfcCraneRailFShapeProfileDef, IfcLShapeProfileDef, IfcRectangleHollowProfileDef, IfcTShapeProfileDef, IfcUShapeProfileDef, IfcZShapeProfileDef_ and _IfcAsymmetricIShapeProfileDef_.
* **Extrusion:** The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the position of the _IfcExtrudedAreaSolid_.

In addition to the full 'SweptSolid' representation a simple representation for the axis of gravity can be used., i.e. as a second _IfcRepresentationMap_. It represents the neutral axis of stress which is not necessarily in the profiles center of gravity. In this case the following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Axis'
* _RepresentationType_ : 'GeometricCurveSet'

**Position number:******  
The position number is specified in the attribute _IfcTypeProduct.Tag_.

**Non geometric profile properties:******  
Non geometric profile properties (for instance mechanical properties) are specified through _IfcProfileProperties_ (and its specific subtypes). These properties are attached to _IfcMemberType_ by the relationship _IfcRelAssociatesProfileProperties_. If an individual occurrence has its own profile property assignment (see _IfcMember_), then this overrides the profile property assignment given at the _IfcMemberType_.

**Quantity related properties:******  
Quantity related properties, which do not relate to the profile, are specified through _IfcElementQuantity_ (and its specific subtypes). These properties are attached to the _IfcMemberType_ by the relationship _IfcRelDefinesByProperties_. If an individual occurrence has its own element quantity assignment (see _IfcMember_), then this overrides the quantity assignment given at the _IfcMemberType_. The following quantities are foreseen, but will be subjected to the local standard of measurement used:

<table cellpadding="2" cellspacing="2" border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i><b>Name</b></i></font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1"><i><b>Description</b></i></font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i><b>Value
			 Type</b></i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">NominalLength</font></td>
		  
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total nominal
			 length of the member, not taking into account any cut-out's or other processing
			 features.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityLength</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">CrossSectionArea</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total area of
			 the cross section (or profile) of the member. The exact definition and
			 calculation rules depend on the method of measurement used.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityArea</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">OuterSurfaceArea</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total area of
			 the extruded surfaces of the member (not taking into account the end cap
			 areas), normally generated as perimeter * length.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityArea</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">TotalSurfaceArea</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total area of
			 the member, normally generated as perimeter * length + 2 * cross section
			 area.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityArea</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">GrossVolume</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total gross
			 volume of the member, not taking into account possible processing features
			 (cut-out's, etc.) or openings and recesses. The exact definition and
			 calculation rules depend on the method of measurement used.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityVolume</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">NetVolume</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1">Total net
			 volume of the member, taking into account possible processing features
			 (cut-out's, etc.) or openings and recesses. The exact definition and
			 calculation rules depend on the method of measurement used.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityVolume</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">GrossWeight</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1"> Total gross
			 weight of the member without add-on parts, not taking into account possible
			 processing features (cut-out's, etc.) or openings and recesses.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityWeight</i></font></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT"><font size="-1">NetWeight</font></td> 
		  <td valign="TOP" align="LEFT" width="60%"><font size="-1"> Total net
			 weight of the member without add-on parts, taking into account possible
			 processing features (cut-out's, etc.) or openings and recesses.</font></td> 
		  <td valign="TOP" align="LEFT"><font size="-1"><i>IfcQuantityWeight</i></font></td> 
		</tr> 
	 </table>