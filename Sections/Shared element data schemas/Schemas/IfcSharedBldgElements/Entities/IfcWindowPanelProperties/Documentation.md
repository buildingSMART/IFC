A description of the window panel. A window panel is a casement, i.e. a component, fixed or opening, consisting essentially of a frame and the infilling. The infilling of a window panel is normally glazing. The way of operation is defined in the operation type.

The _IfcWindowPanelProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcWindowStyle_. More information about the window panel can be included in the same list of the IfcWindowStyle using the _IfcPropertySet_ for dynamic extensions.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
		Release 2.0, it had been renamed from IfcWindowPanel in IFC Release
		2x.</font>

****Geometry Use Definitions****

The _IfcWindowPanelProperties_ does not hold an own geometric representation. However it defines parameter, which can be used to create the shape of the _IfcWindowStyle_ (which is inserted by the _IfcWindow_ into the spatial context of the project).

**Interpretation of parameter**

The parameters at the _IfcWindowPanelProperties_ define a standard window panel. The outer boundary of the panel is determined by the occurrence parameter assigned to the IfcWindow, which inserts the IfcWindowStyle. It has to take the lining parameter into account as well. The position of the window panel within the overall window is determined by the _PanelPosition_ attribute.

<table border="1" cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><img src="figures/ifcwindowpanelproperties-fig01.gif" alt="panel 1" width="239" height="129" border="0"></td> 
		  <td valign="TOP" align="LEFT">The panel is applied to the position
			 within the lining, as defined by the panel position attribute. The following
			 parameter apply to that panel: 
			 <ul> 
				<li><i>FrameDepth</i></li> 
				<li><i>FrameThickness</i></li> 
			 </ul></td> 
		</tr> 
	 </table>
