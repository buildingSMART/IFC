**Definition from ISO/DIS 10303-42:1999(E)**: A surface curve swept area solid is a type of swept area solid which is the result of sweeping a face along a _Directrix_ lying on a _ReferenceSurface_. The orientation of the _SweptArea_ is related to the direction of the surface normal.

The _SweptArea_ is required to be a curve bounded surface lying in the plane z = 0 and this is swept along the _Directrix_ in such a way that the origin of the local coordinate system used to define the _SweptArea_ is on the _Directrix_ and the local x-axis is in the direction of the normal to the _ReferenceSurface_ at the current point. The resulting solid has the property that the cross section of the surface by the normal plane to the _Directrix_ at any point is a copy of the _SweptArea_.

The orientation of the _SweptArea_ as it sweeps along the _Directrix_ is precisely defined by a _CartesianTransformationOperator3d_ with attributes:

* _LocalOrigin_ as point (0; 0; 0), 
* _Axis1_ as the normal N to the _ReferenceSurface_ at the point of the _Directrix_ with parameter u. 
* _Axis3_ as the direction of the tangent vector t at the point of the _Directrix_ with parameter u.   The remaining attributes are defaulted to define a corresponding transformation matrix T(u), which varies with the _Directrix_ parameter u. 

> <font size="-1">NOTE: The geometric shape of the solid is not
		dependent upon the curve parameterization; the volume depends upon the area
		swept and the length of the <i>Directrix</i>. </font>

The swept face is given by _IfcProfileDef_ (or subtypes), the profile definition is given within a 2D coordinate system, which is inserted into the XY plane of the _Position_ coordinate system inherited from the supertype _IfcSweptAreaSolid_. The attributes of the _CartesianTransformationOperator3d_ (as given above) should apply to the _Position_ coordinate system, in which the profile is inserted.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP
		entity: surface_curve_swept_area_solid. Please refer to ISO/DIS
		10303-42:1999(E), p. 274 for the final definition of the formal
		standard.</font>

> <font size="-1" color="#0000FF">HISTORY: New entity in Release
		IFC2x Edition 2.</font>

Informal propositions:

1.  The _SweptArea_ shall lie in the plane z = 0. 
2.  The directrix shall lie on the _ReferenceSurface_.