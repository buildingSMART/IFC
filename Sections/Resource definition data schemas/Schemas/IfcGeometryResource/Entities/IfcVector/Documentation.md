**Definition from ISO/CD 10303-42:1992**: The vector is defined in terms of the direction and magnitude of the vector. The value of the magnitude attribute defines the magnitude of the vector.

> <font size="-1">NOTE: The magnitude of the vector can not be reliable
		  calculated from the components of the Orientation attribute. This form of
		  representation was selected to reduce problems with numerical instability. For
		  example a vector of magnitude 2.0 mm and equally inclined to the coordinate
		  axes could be represented with Orientation attribute of (1.0,1.0,1.0).
		  </font>
>

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  vector. Please refer to ISO/IS 10303-42:1994, p.27 for the final definition of
		  the formal standard. The derived attribute <i>Dim</i> has been added (see also
		  note at <i>IfcGeometricRepresentationItem</i>).</font>
> 
> <font size="-1" color="#0000FF">HISTORY: New entity in IFC Release 1.0
		  </font>
>