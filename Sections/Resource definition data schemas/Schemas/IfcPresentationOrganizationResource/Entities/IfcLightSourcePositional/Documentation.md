**Definition from ISO/CD 10303-46:1992**: The light source positional entity is a subtype of light source. This entity has a light source position and attenuation coefficients. A positional light source affects a surface based on the surface's orientation and position.

**Definition from ISO/IEC 14772-1:1997**: The Point light node specifies a point light source at a 3D location in the local coordinate system. A point light source emits light equally in all directions; that is, it is omnidirectional. Point light nodes are specified in the local coordinate system and are affected by ancestor transformations.

Point light node's illumination falls off with distance as specified by three attenuation coefficients. The attenuation factor is

> <font size="-1">1/max(attenuation[0] + attenuation[1] &times; r +
		  attenuation[2] &times; r 2 , 1), </font>
>

where r is the distance from the light to the surface being illuminated. The default is no attenuation. An attenuation value of (0, 0, 0) is identical to (1, 0, 0). Attenuation values shall be greater than or equal to zero.

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP entity:
		  light_source_positional. Please refer to ISO/IS 10303-46:1994, p. 32 for the
		  final definition of the formal standard. </font>
> 


> <font color="#0000FF" size="-1">NOTE: In addition to the
		attributes as defined in ISO10303-46 the additional property from ISO/IEC
		14772-1:1997 (VRML) <i>Radius</i> and <i>QuadricAttenuation</i> are added to
		this subtype and the <i>AmbientIntensity</i> and <i>Intensity</i> are inherited
		from the supertype.</font>

> <font color="#0000FF" size="-1">HISTORY: This is a new entity
		in IFC 2x, renamed and enhanced in IFC2x2.</font>