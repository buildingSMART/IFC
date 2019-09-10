An _IfcPresentationLayerAssignmentWithStyle_ extends the presentation layer assignment with capabilities to define visibility control, access control and common style information.

The visibility control allows to define a layer to be either 'on' or 'off', and/or 'frozen' or 'not&nbsp;frozen'. The access control allows to block graphical entities from manipulations by setting a layer to be either 'blocked' or 'not blocked'. Common style information can be given to the layer.

> <small>NOTE &nbsp;Style information assigned to
layers is often
restricted to 'layer colour', 'curve font', and/or 'curve width'. These
styles are assigned by using the <i>IfcCurveStyle</i>
within the <i>LayerStyles</i>.<br>
  <br>
NOTE: If a styled item
is assigned to a layer using the <i>IfcPresentationLayerAssignmentWithStyle</i>,
it inherits the style information from the layer. In this case, it
should omit its own style information. If the styled item has style
information assigned (e.g. by <i>IfcCurveStyle,
IfcFillAreaStyle, IfcTextStyle, IfcSurfaceStyle, IfcSymbolStyle</i>),&nbsp;
then it overrides the style provided by the <i>IfcPresentationLayerAssignmentWithStyle</i>.</small>

> <font color="#0000ff"><small> NOTE&nbsp;
The <i>IfcPresentationLayerAssignmentWithStyle</i> extends
the presentation_layer_assignment entity as defined in ISO/IS
10303-46:1994, p. 36.</small> </font>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in Release IFC2x 2nd Edition.</font><br>
  <font color="#ff0000">IFC2x Edition 3 CHANGE
&nbsp;The attributes have been modified without upward
compatibility.</font>
  </small>
