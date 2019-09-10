**Definition from BS 6100**: A permeable covering is a permeable cover for an opening which allows airflow .

A description of a panel within a door or window (as fillers for opening) which allows for air flow. It is given by its properties (_IfcPermeableCoveringProperties_). A permeable covering is a casement, i.e. a component, fixed or opening, consisting essentially of a frame and the infilling. The infilling is normally a grill, a louver or a screen. The way of operation is defined in the operation type.

The _IfcPermeableCoveringProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcWindowStyle_ or the _IfcDoorStyle_. More information about the permeable covering can be included in the same list of the window or door style using the _IfcPropertySet_ for dynamic extensions. This particularly applies for additional properties for the various operation types

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
		Release 2.0, it had been renamed from <i>IfcPermeableCovering</i> in IFC
		Release 2x.</font>

****Geometry Use Definitions****

The _IfcPermeableCoveringProperties_ does not hold an own geometric representation. However it defines parameter, which can be used to create the shape of the _IfcWindowStyle_ (which is inserted by the _IfcWindow_ into the spatial context of the project), or of the _IfcDoorStyle_ (which is inserted by the _IfcDoor_).

**Interpretation of parameter**

The parameters at the _IfcPermeableCoveringProperties_ define a standard permeable covering. The outer boundary of the panel is determined by the occurrence parameter assigned to the _IfcWindow_ or _IfcDoor_. It has to take the lining parameter into account as well. The position of the permeable covering within the overall window or door is determined by the _PanelPosition_ attribute.

<table border="1" cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><img src="figures/ifcpermeablecoveringproperties.gif" alt="covering" width="400" height="215" border="0"></td> 
		  <td valign="TOP" align="LEFT">The panel is applied to the position
			 within the lining, as defined by the panel position attribute. The following
			 parameter apply to that panel: 
			 <ul> 
				<li>FrameDepth</li> 
				<li>FrameThickness</li> 
			 </ul></td> 
		</tr> 
	 </table>
