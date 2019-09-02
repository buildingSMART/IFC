_IfcSurfaceStyleLighting_ is a container class for properties for calculation of physically exact illuminance related to a particular surface style.

![material reflection components](figures/IfcSurfaceLightingProperties_Fig1.gif)The illustration above shows the reflection and transmission components from an incident ray. The sum of the components for reflection and transmission is a value of 1.0 denoting that the incident ray is completely decomposed into reflection and transmission components. Each value of reflection and transmission is therefore within the range 0.0 to 1.0.

All these factors can be measured physically and are ratios for the red, green and blue part of the light. These properties are defined in the model as Type _IfcColorRGB_ with a factor for each colour.

> <font size="-1">EXAMPLE: A green glass transmits only green light, so
		  its transmission factor is 0.0 for red, between 0.0 and 1.0 for green and 0.0
		  for blue. A green surface reflects only green light, so the reflectance factor
		  is 0.0 for red, between 0.0 and 1.0 for green and 0.0 for blue.
		  </font>
>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC 2x
		Edition 2.</font>