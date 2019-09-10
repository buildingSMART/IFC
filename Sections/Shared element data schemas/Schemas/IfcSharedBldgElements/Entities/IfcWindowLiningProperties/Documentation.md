The window lining is the frame which enables the window to be fixed in position. The window lining is used to hold the window panels or other casements. The parameter of the window lining (_IfcWindowLiningProperties_) define the geometrically relevant parameter of the lining.

The _IfcWindowLiningProperties_ are included in the list of properties (_HasPropertySets_) of the _IfcWindowStyle_. More information about the window lining can be included in the same list of the _IfcWindowStyle_ using the _IfcPropertySet_ for dynamic extensions.

> <font color="#0000FF" size="-1">HISTORY New Entity in IFC
		Release 2.0. Has been renamed from <i>IfcWindowLining</i> in IFC Release 2x.
		</font>

****Geometry Use Definitions****

The _IfcWindowLiningProperties_ does not hold an own geometric representation. However it defines parameter, which can be used to create the shape of the window style (which is inserted by the _IfcWindow_ into the spatial context of the project).

**Interpretation of parameter**

The parameters at the _IfcWindowLiningProperties_ define a standard window lining, including (if given) a mullion and a transom (for horizontal and vertical splits). The outer boundary of the lining is determined by the occurrence parameter assigned to the _IfcWindow_, which inserts the _IfcWindowStyle_.

<table border="1" cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td><img src="figures/ifcwindowliningproperties-fig05.gif" alt="lining 5" width="219" height="140" border="0"></td> 
		  <td valign="TOP" align="LEFT">The lining is applied to all faces of the
			 opening reveal. The parameter are: 
			 <ul> 
				<li><i>LiningDepth</i></li> 
				<li><i>LiningThickness</i></li> 
			 </ul></td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcwindowliningproperties-fig01.gif" alt="lining 1" width="209" height="233" border="0"></td> 
		  <td valign="TOP" align="LEFT">If the <i>OperationType</i> of the window
			 style is 
			 <ul> 
				<li>DoublePanelVertical (shown)</li> 
				<li>TriplePanelBottom</li> 
				<li>TriplePanelTop</li> 
				<li>TriplePanelLeft</li> 
				<li>TriplePanelRight</li> 
			 </ul>the following additional parameter apply: 
			 <ul> 
				<li><i>MullionThickness</i></li> 
				<li><i>FirstMullionOffset</i> - measured as offset to the Z axis
				  (in XZ plane)</li> 
			 </ul> </td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcwindowliningproperties-fig02.gif" alt="lining 2" width="233" height="209" border="0"></td> 
		  <td valign="TOP" align="LEFT">If the <i>OperationType</i> of the window
			 style is 
			 <ul> 
				<li>DoublePanelHorizontal</li> 
				<li>TriplePanelBottom</li> 
				<li>TriplePanelTop</li> 
				<li>TriplePanelLeft</li> 
				<li>TriplePanelRight</li> 
			 </ul>the following additional parameter apply 
			 <ul> 
				<li><i>TransomThickness</i> </li> 
				<li><i>FirstTransomOffset</i> measured as offset to the X axis (in
				  XZ plane)</li> 
			 </ul></td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcwindowliningproperties-fig03.gif" alt="lining 3" width="303" height="261" border="0"></td> 
		  <td valign="TOP" align="LEFT">If the <i>OperationType</i> of the window
			 style is 
			 <ul> 
				<li><i>TriplePanelVertical</i></li> 
			 </ul>the following additional parameter apply 
			 <ul> 
				<li><i>SecondMullionOffset</i></li> 
			 </ul></td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcwindowliningproperties-fig04.gif" alt="lining 4" width="261" height="303" border="0"></td> 
		  <td valign="TOP" align="LEFT">If the <i>OperationType</i> of the window
			 style is 
			 <ul> 
				<li><i>TriplePanelHorizontal</i></li> 
			 </ul>the following additional parameter apply 
			 <ul> 
				<li><i>SecondTransomOffset</i></li> 
			 </ul></td> 
		</tr> 
	 </table>

NOTE

1. All offsets are given as a normalized ratio measure.