An _IfcPresentationLayerAssignmentWithStyle_ extends the presentation layer assignment with capabilities to define visibility control, access control and common style information.

The visibility control allows to define a layer to be either 'on' or 'off', and/or 'frozen' or 'not frozen'. The access control allows to block graphical entities from manipulations by setting a layer to be either 'blocked' or 'not blocked'. Common style information can be given to the layer.

> NOTE&nbsp; Style information assigned to layers is often restricted to 'layer colour', 'curve font', and/or 'curve width'. These styles are assigned by using the _IfcCurveStyle_ within the _LayerStyles_.

> NOTE&nbsp; If a styled item is assigned to a layer using the _IfcPresentationLayerAssignmentWithStyle_, it inherits the style information from the layer. In this case, it should omit its own style information. If the styled item has style information assigned (such as by _IfcCurveStyle_, _IfcFillAreaStyle_, _IfcTextStyle_, _IfcSurfaceStyle_, _IfcSymbolStyle_), then it overrides the style provided by the _IfcPresentationLayerAssignmentWithStyle_.

> NOTE&nbsp; The _IfcPresentationLayerAssignmentWithStyle_ extends the presentation_layer_assignment entity as defined in ISO/IS 10303-46:1994, p. 36.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x3}
> IFC2x3 CHANGE &nbsp;The attributes have been modified without upward compatibility.