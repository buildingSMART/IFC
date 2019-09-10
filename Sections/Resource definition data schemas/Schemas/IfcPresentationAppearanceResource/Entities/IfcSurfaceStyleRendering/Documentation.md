_IfcSurfaceStyleRendering_ holds the properties for visualization related to a particular surface side style.

It allows rendering properties to be defined by:

* a transparency component (_Transparency_ attribute)
* a colour component (_SurfaceColour_ attribute inherited from _IfcSurfaceStyleShading_)
* a reflectance component, given either by 
    * applying reflectance factors to the surface colour: 
        * diffuse component (_SurfaceColour \* DiffuseFactor_)
        * transmission component (_SurfaceColour \* TransmissionFactor_ )
        * diffuse transmission component (_SurfaceColour \* DiffuseTransmissionFactor_)
        * reflection component (_SurfaceColour \* ReflectionFactor_)
        * specular component (_SurfaceColour \* SpecularFactor_ attribute together with _SpecularHighlight_) 
    * explicitly defining such factors as colours (_DiffuseColour_, _TransmissionColour_, _DiffuseTransmissionColour_, _ReflectionColour_ and _SpecularColour_) 
* a displacement component, currently only given by a texture map with the TextureType = bump
* a coverage component, currently only given by the alpha component of the texture map (2 or 4 component colour texture)

> <font size="-1">NOTE: The inherited attribute
		<i>SurfaceColour</i> is treated as the ambient colour and specifies how much
		ambient light from light sources this surface shall reflect. Ambient light is
		omnidirectional and depends only on the number of light sources, not their
		positions with respect to the surface.</font>

> <font size="-1">NOTE: If the reflectance method, as given by the
		  <i>IfcReflectanceMethodEnum</i> is "GLASS", the transmission factor controls
		  the level of transparency in the glass, In this case the transparency factor is
		  interpreted as transmission factor.</font>
>

> <font size="-1">NOTE: Both <i>Transparency</i> and
		<i>TransmissionColour</i> (or factor) are included, the following definitions
		apply</font><ul> 
		  <li><font size="-1">Transparency is the ratio of the transmitted flux
			 in a solid angle of 2 * PI sr (one hemisphere). It is a simple colour
			 filtration that does not account for refraction. </font></li> 
		  <li><font size="-1">Transmission factor of a material is the ratio of
			 transmitted flux in a given solid angle to the transmitted flux of a completely
			 diffuse material with 100% transmission in the same solid angle. It is the
			 portion of light that goes through the material and may be
			 refracted.</font></li> 
		</ul>

> <font color="#0000FF"><font size="-1">NOTE: IFC 2x Edition 2
		adds additional capability for presentation of physically accurate illuminance
		on surfaces. VRML type rendering and rendering based on ISO 10303-46 continues
		to be supported by a subset of the information. For reflectance equations and
		further information about the surface style properties and its processing, see:
		</font> </font><ul> 
		  <li><font size="-1" color="#0000FF">ISO/IEC 14772-1: 1997: The Virtual
			 Reality Modeling Language</font></li> 
		</ul>

> <font size="-1" color="#0000FF">NOTE: The definition of
		<i>IfcSurfaceStyleRenderingProperties</i> includes the definitions as found in
		ISO 10303-46:1994, in particular of: </font>> * <font size="-1" color="#0000FF">surface_style_rendering_with_properties</font>
> * <font size="-1" color="#0000FF">surface_style_rendering_ambient</font>
> * <font size="-1" color="#0000FF">surface_style_rendering_ambient_diffuse</font>
> * <font size="-1" color="#0000FF">surface_style_rendering_ambient_diffuse_specular</font>
> * <font size="-1" color="#0000FF">surface_style_transparent</font>

> <font size="-1" color="#0000FF">In addition to the attributes
		as defined in ISO 10303-46, i.e. ambient_reflectance, diffuse_reflectance,
		specular_reflectance, specular_exponent, and specular_colour, the current IFC
		definition adds other colours, reflectance factors and specular
		roughness..</font>

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x.</font>