**Definition from ISO/CD 10303-46:1992**: The surface style element select is a selection of the different surface styles to use in the presentation of the side of a surface.

The select type only includes the _IfcSurfaceStyleRendering_ (which is the equivalent to surface_style_rendering) from the select type surface_style_element_select. In addition it has the _IfcSurfaceStyleLighting_, which holds the exact physically based lighting properties for lighting based calculation algorithms (as the opposite to the rendering based calculation), the _IfcSurfaceStyleRefraction_ (for more advanced refraction indices) and _IfcSurfaceStyleWithTextures_ (to allow for image textures applied to surfaces). In addition an _IfcExternallyDefinedSurfaceStyle_ can be selected that points into an external material library.

> <font size="-1">NOTE The <i>IfcSurfaceLightingProperties</i> are
		  needed for exact lighting calculation, because physically based lighting
		  calculation algorithms need exact physically based parameters. The factors in
		  <i>IfcSurfaceStyleRendering</i> lack the physical base, they are intended for
		  rendering calculations, but a lighting calculation based software cannot use
		  these values.</font>
>

> <font size="-1" color="#0000FF">NOTE: Corresponding STEP type:
		  surface_style_element_select. Please refer to ISO/IS 10303-46:1994, p. 85 for
		  the final definition of the formal standard. </font>
> 


> <font size="-1" color="#0000FF">HISTORY: New Select type in
		IFC Release 2x2. </font>