_IfcSurfaceStyleRefraction_ extends the surface style lighting, or the surface style rendering definition for properties for calculation of physically exact illuminance by adding seldomly used properties. Currently this includes the refraction index (by which the light ray refracts when passing through a prism) and the dispersion factor (or Abbe constant) which takes into account the wavelength dependency of the refraction.

> <font size="-1">NOTE: If such refraction properties are used,
		the <i>IfcSurfaceStyle</i> should include within its set of <i>Styles</i>
		(depending on whether rendering or lighting is used) an instance of
		<i>IfcSurfaceStyleLighting</i> and <i>IfcSurfaceStyleRefraction</i>, or an
		instance of <i>IfcSurfaceStyleRendering</i> and
		<i>IfcSurfaceStyleRefraction</i>.</font>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC 2x
		Edition 2.</font>