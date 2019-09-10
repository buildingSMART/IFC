A slender timber, concrete, or steel structural element, driven, jetted, or otherwise embedded on end in the ground for the purpose of supporting a load.

> <font color="#0000FF" size="-1"> HISTORY New entity in IFC
		Release 2x2 </font>

**Geometry Use Definitions:**

The geometric representation of _IfcPile_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation. Included are:

**Local Placement**  
The local placement for _IfcPile_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**Standard Geometric Representation using Swept Solid
		Representation**  
The standard geometric representation of _IfcPile_ is defined using the swept solid representation. The _RepresentationType_ attribute of _IfcShapeRepresentation_ should have the value 'SweptSolid'. The following constraints apply to the standard representation:

* **Solid:** _IfcExtrudedAreaSolid_ shall be supported 
* **Profile:** _IfcRectangleProfileDef_ and _IfcCircleProfileDef_ shall be supported 
* **Extrusion:** The profile shall be extruded vertically, i.e., in the direction of the z-axis of the co-ordinate system of the referred spatial structure element. It might be further constraint to be in the direction of the global z-axis in implementers agreements. The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the Position of the _IfcExtrudedAreaSolid_. 

**Advanced Geometric Representation using CSG Representation**  
The advanced geometric representation of _IfcPile_ is defined using the Swept Solid or CSG representation. The _RepresentationType_ attribute of _IfcShapeRepresentation_ should have the value 'SweptSolid' or 'CSG'. The following additional constraints apply to the advanced representation:

* **Solid:** see standard geometric representation, 
* **Profile:** _IfcRectangleProfileDef_, _IfcCircleProfileDef_, _IfcIShapeProfileDef_ and _IfcArbitraryProfileDef_ shall be supported. 
* **Extrusion:** All extrusion directions shall be supported 
* **Boolean result:** The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_.
