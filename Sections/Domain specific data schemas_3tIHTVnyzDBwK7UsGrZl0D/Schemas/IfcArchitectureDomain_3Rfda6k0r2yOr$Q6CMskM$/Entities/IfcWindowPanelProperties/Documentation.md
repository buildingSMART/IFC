A window panel is a casement, that is, a component, fixed or opening, consisting essentially of a frame and the infilling. The infilling of a window panel is normally glazing. The way of operation is defined in the operation type.

The _IfcWindowPanelProperties_ are used to parametrically describe the shape and operation of window panels. The parametric definition can be added solely or additionally to the explicit shape representation of the window.

The _IfcWindowStyle_ can define windows consisting of more then one panel. In this case, one instance of _IfcWindowPanelProperties_ has to be included for each window panel. The _PanelPosition_ attribute, in conjunction with the _IfcWindowStyle.OperationType_ attribute, determines to which panel the _IfcWindowPanelProperties_apply.

The _IfcWindowPanelProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcWindowStyle_. More information about the window panel can be included in the same list of the _IfcWindowStyle_ using the _IfcPropertySet_ for dynamic extensions.

> HISTORY&nbsp; New entity in IFC2.0, it had been renamed from IfcWindowPanel in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Supertype changed to new _IfcPreDefinedPropertySet_.

{ .use-head}
Geometry use definitions

The _IfcWindowPanelProperties_ does not hold an own geometric representation. However it defines parameter, which can be used to create the shape of the _IfcWindowType_ (which is inserted by the _IfcWindow_ into the spatial context of the project).

The parameters at the _IfcWindowPanelProperties_ define a standard window panel. The outer boundary of the panel is determined by the occurrence parameter assigned to the IfcWindow, which inserts the IfcWindowStyle. It has to take the lining parameter into account as well. The position of the window panel within the overall window is determined by the _PanelPosition_ attribute.

As shown in Figure 1, the panel is applied to the position within the lining as defined by the panel position attribute. The following parameter apply to that panel: _FrameDepth_, _FrameThickness_.

!["panel 1"](../../../figures/IfcWindowPanelProperties-Fig01.gif "Figure 1 &mdash; Window panel properties")