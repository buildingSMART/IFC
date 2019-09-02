The window style defines a particular style of windows, which may be included into the spatial context of the building model through an (or multiple) instances of _IfcWindow_. A window style defines the overall parameter of the window style and refers to the particular parameter of the lining and one (or several) panels through the _IfcWindowLiningProperties_ and the _IfcWindowPanelProperties_.

The window entity (_IfcWindow_) defines a particular occurrence of a window inserted in the spatial context of a project. The actual parameter of the window and/or its shape is defined at the _IfcWindowStyle_, to which the _IfcWindow_ related by the inverse relationship _IsDefinedBy_ pointing to _IfcRelDefinesByType_. The _IfcWindowStyle_ also defines the particular attributes for the lining (_IfcWindowLiningProperties_) and panels (_IfcWindowPanelProperties_).

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
		Release 2x.</font>

> <font color="#FF0000" size="-1">IFC2x2 COMPATIBILITY NOTICE:
		The entity <i>IfcWindowStyle</i> is still subtyped from the
		<i>IfcTypeProduct</i> to provide upward compatibility. This is a recorded
		anomaly as all other types for building elements are now subtyped from
		<i>IfcBuildingElementType</i> and have the suffix "Type", not "Style".</font>

****Geometry Use Definitions****:

The _IfcWindowStyle_ defines the baseline geometry, or the representation map, for all occurrences of the window style, given by the IfcWindow, pointing to this style. The representation of the window style may be given by the agreed set of minimal parameters, defined for the window lining and the window panel(s), or it my be given by a geometric representation used by the _IfcRepresentationMap_. The attribute _ParameterTakesPrecedence_ decides, whether the set of parameters can be used to exactly represent the shape of the window style (TRUE), or whether the attached _IfcRepresentationMap_ holds the exact representation (FALSE).

**Interpretation of parameters**

The _IfcWindowStyleOperationTypeEnum_ defines the general layout of the window style. Depending on the enumerator, the appropriate instances of _IfcWindowLiningProperties_ and _IfcWindowPanelProperties_ are attached in the list of _HasPropertySets_. See geometry use definitions there.