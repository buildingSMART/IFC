This enumeration defines the basic configuration of the window type in terms of the number of window panels and the subdivision of the total window. The window configurations are given for windows with one, two or three panels (including fixed panels).

Windows which are subdivided into more than three panels have to be defined by the geometry only. The type of such windows is USERDEFINED.

> <font color="#0000FF" size="-1">HISTORY New Enumeration in IFC
		Release 2.0.</font>

**Illustration**

<table border="1"> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT"><i>Enumerator</i></td> 
		  <td width="46%" valign="TOP" align="LEFT"><i>Description</i></td> 
		  <td width="23%" valign="TOP" align="LEFT"><i>Figure</i></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">SinglePanel</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with one
			 panel.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig01.gif" width="58" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">DoublePanelVertical</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with two panels. The
			 configuration of the panels is vertically.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig02.gif" width="115" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">DoublePanelHorizontal</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with two panels. The
			 configuration of the panels is horizontally.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig03.gif" width="115" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelVertical</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of the panels is vertically.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig04.gif" width="171" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelHorizontal </td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of the panels is horizontally.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig05.gif" width="115" height="171" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelBottom</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of two panels is vertically and the third one is horizontally at
			 the bottom.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig06.gif" width="115" height="171" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelTop</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of two panels is vertically and the third one is horizontally at
			 the top.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig07.gif" width="115" height="171" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelLeft</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of two panels is horizontally and the third one is vertically at
			 the left hand side.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig08.gif" width="171" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">TriplePanelRight</td> 
		  <td width="46%" valign="TOP" align="LEFT">Window with three panels. The
			 configuration of two panels is horizontally and the third one is vertically at
			 the right hand side.<br></td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/ifcwindowstyleoperationenum-fig09.gif" width="171" height="115" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT"> UserDefined</td> 
		  <td width="46%" valign="TOP" align="LEFT">user defined operation
			 type</td> 
		  <td width="23%" valign="TOP" align="LEFT">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">NotDefined</td> 
		  <td width="46%" valign="TOP" align="LEFT">&nbsp;</td> 
		  <td width="23%" valign="TOP" align="LEFT">&nbsp;</td> 
		</tr> 
	 </table>

NOTE

1. The way how each panel operates is defined at the_IfcWindowPanelProperties.OperationType_.
2. The reference from the window panel to the location of that panel in the window style configuration is handled by the _IfcWindowPanelProperties.PanelPosition_.
3. The figures are shown as elevations in the XZ plane of the local placement of the window, looking into the direction of the positive Y axis.
4. These figures are only shown as illustrations
