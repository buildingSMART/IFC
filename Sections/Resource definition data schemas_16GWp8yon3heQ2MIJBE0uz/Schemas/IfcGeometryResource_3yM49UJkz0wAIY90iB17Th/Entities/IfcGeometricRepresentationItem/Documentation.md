**Definition from ISO/CD 10303-43:1992**: An geometric representation item is a representation item that has the additional meaning of having geometric position or orientation or both. This meaning is present by virtue of:

* being a Cartesian point or a direction 
*  referencing directly a Cartesian point or direction 
* referencing indirectly a Cartesian point or direction 

An indirect reference to a Cartesian point or direction means that a given geometric item references the Cartesian point or direction through one or more intervening geometry or topology items.

> <font size="-1">EXAMPLE: Consider a circle. It gains its geometric
		  position and orientation by virtue of a reference to axis2_placement
		  (IfcAxis2Placement) that is turn references a cartesian_point
		  (IfcCartesianPoint) and several directions (IfcDirection). <br>EXAMPLE:
		  Consider a manifold brep. A manifold_solid_brep (<i>IfcManifoldSolidBrep</i>)
		  is a geometric_representation_item (<i>IfcGeometricRepresentationItem</i>) that
		  through several layers of topological_representation_item's
		  (<i>IfcTopologicalRepresentationItem</i>) references poly loops
		  (<i>IfcPolyLoop</i>). Through additional intervening entities poly loops
		  reference cartesian_point's (<i>IfcCartesianPoint</i>).
		  </font>
>

The derivation of the dimensionality of the _IfcGeometricRepresentationItem_ is different to STEP, there is a specific derived attribute at each class that defines the dimensionality, whereas STEP does it for the representation_context and requires all geometric_representation_item's to have the same dimensionality therein.

The definition of swept area solids as geometric representation items is different to STEP, it is based on a set of predefined profiles (or cross sections), i.e. a set of parameterized geometric primitives widely supported in the industry. Those profiles are used to create volumes through extrusion, revolution and cross section based sweep operations. This method was called attribute driven geometric representation and it was formerly known as implicit geometry in IFC.

> <font color="#0000FF" size="-1">NOTE: Corresponding STEP entity:
		  geometric_representation_item. Please refer to ISO/IS 10303-42:1994, p. 22 for
		  the final definition of the formal standard. The following changes have been
		  made: It does not inherit from ISO/IS 10303-43:1994 entity representation_item.
		  The derived attribute Dim is demoted to the appropriate subtypes. The WR1 has
		  not been incorporated. Not all subtypes that are in ISO/IS 10303-42:1994 have
		  been added to the current IFC Release . </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.5</font>
>