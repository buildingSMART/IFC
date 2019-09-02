A steel element such as a wire, cable, bar, rod, or strand used to impart prestress to concrete when the element is tensioned.

> <font color="#0000FF" size="-1"> HISTORY New entity in IFC
		Release 2x2 </font>

**Geometry Use Definitions:**

The geometric representation of _IfcTendon_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The use of local placement is defined at the supertype _IfcBuildingElementComponent_.

**Standard Geometric Representation using Swept Solid
		Representation**  
The standard geometric representation of _IfcTendon_ is defined using the swept solid representation. The _RepresentationType_ attribute of _IfcShapeRepresentation_ should have the value 'SweptSolid'. The solid is formed from a cross section approximated as a circular disk swept along any arbitrary curve. Given this, the following constraints apply to the standard representation:

* **Solid:** _IfcSweptDiskSolid_ introduced in IFC Release 2x2 shall be supported. 
* **Profile:** The circular disk cross section approximation is defined by the _Radius_ attribute of _IfcSweptDiskSolid_. 
* **Extrusion:** The extrusion along any arbitrary curve is defined by the _Directrix_ attribute of _IfcSweptDiskSolid_. 

**Simplified Geometric Representation**  
Simplified geometric representations may be used based on local agreements.