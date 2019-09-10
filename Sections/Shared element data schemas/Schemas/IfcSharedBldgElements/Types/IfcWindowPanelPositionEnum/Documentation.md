This enumeration defines the basic configuration of the window type in terms of the location of window panels. The window configurations are given for windows with one, two or three panels (including fixed panels). It corresponds to the _OperationType_ of the _IfcWindowStyle_ definition, which references the _IfcWindowPanelProperties_.

Windows which are subdivided into more than three panels have to be defined by the geometry only. The type of such windows is given by an _IfcWindowStyle.OperationType_ = USERDEFINED or NOTDEFINED (see _IfcWindowStyleOperationEnum_ for details).

> <font color="#0000FF" size="-1">HISTORY New Enumeration in IFC
		Release 2.0.</font>

**Illustration**

<table border="1"> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT"><i>Enumerator from
			 IfcWindowStyleOperationEnum</i></td> 
		  <td width="30%" valign="TOP" align="LEFT"><i>Use of enumerators from
			 IfcWindowPanelPositionEnum</i></td> 
		  <td width="23%" valign="TOP" align="LEFT"><i>Figure</i></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">DoublePanelVertical</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = LEFT<br>second
			 IfcWindowPanelProperties with PanelPosition = RIGHT</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig01.gif" width="152" height="151" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT" height="154">DoublePanelHorizontal</td> 
		  <td width="30%" valign="TOP" align="LEFT" height="154">first
			 IfcWindowPanelProperties with PanelPosition = TOP<br>second
			 IfcWindowPanelProperties with PanelPosition = BOTTOM</td> 
		  <td width="23%" valign="TOP" align="LEFT" height="154"><img src="figures/ifcwindowpanelpositionenum-fig02.gif" width="152" height="151" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelVertical</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = LEFT<br>second
			 IfcWindowPanelProperties with PanelPosition = MIDDLE<br>third
			 IfcWindowPanelProperties with PanelPosition = RIGHT</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig03.gif" width="209" height="152" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelHorizontal </td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = TOP<br>second
			 IfcWindowPanelProperties with PanelPosition = MIDDLE<br>third
			 IfcWindowPanelProperties with PanelPosition = BOTTOM</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig04.gif" width="151" height="208" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelBottom</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = LEFT<br>second
			 IfcWindowPanelProperties with PanelPosition = RIGHT<br>third
			 IfcWindowPanelProperties with PanelPosition = BOTTOM</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig05.gif" width="151" height="208" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelTop</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = TOP<br>second
			 IfcWindowPanelProperties with PanelPosition = LEFT<br>third
			 IfcWindowPanelProperties with PanelPosition = RIGHT</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig06.gif" width="151" height="208" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelLeft</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = LEFT<br>second
			 IfcWindowPanelProperties with PanelPosition = TOP<br>third
			 IfcWindowPanelProperties with PanelPosition = BOTTOM</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig07.gif" width="209" height="152" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelRight</td> 
		  <td width="30%" valign="TOP" align="LEFT">first
			 IfcWindowPanelProperties with PanelPosition = TOP<br>second
			 IfcWindowPanelProperties with PanelPosition = BOTTOM<br>third
			 IfcWindowPanelProperties with PanelPosition = RIGHT</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowpanelpositionenum-fig08.gif" width="209" height="152" border="0"></td> 
		</tr> 
	 </table>

NOTE

1. The figures are shown as elevations in the XZ plane of the local placement of the window, looking into the direction of the positive Y axis.
2. These figures are only shown as illustrations.
