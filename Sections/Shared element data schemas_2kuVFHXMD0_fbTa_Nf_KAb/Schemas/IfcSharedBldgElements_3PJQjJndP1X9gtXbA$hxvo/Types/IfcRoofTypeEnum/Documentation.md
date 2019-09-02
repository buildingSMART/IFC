This enumeration defines the basic configuration of the roof in terms of the different roof shapes.

Roofs which are subdivided into more than these basic shapes have to be defined by the geometry only. Also roofs with non-regular shapes (free form roof ) have to be defined by the geometry only. The type of such roofs is FREEFORM.

> <font color="#0000FF" size="-1">HISTORY New Enumeration in IFC
		Release 2x.</font>

**Illustration**

<table border="1"> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT"><i>Enumerator</i></td> 
		  <td width="46%" valign="TOP" align="LEFT"><i>Description</i></td> 
		  <td width="23%" valign="TOP" align="LEFT"><i>Figure</i></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">FLAT_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having no slope, or
			 one with only a slight pitch so as to drain rainwater.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig01-FlatRoof.gif" alt="FlatRoof" width="242" height="143" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">SHED_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having a single
			 slope.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig02-ShedRoof.gif" alt="ShedRoof" width="236" height="189" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">GABLE_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof sloping downward in
			 two parts from a central ridge, so as to form a gable at each end.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig03-GableRoof.gif" alt="GableRoof" width="233" height="155" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">HIP_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having sloping ends
			 and sides meeting at an inclined projecting angle.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig04-HipRoof.gif" alt="HipRoof" width="242" height="143" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">HIPPED_GABLE_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having a hipped end
			 truncating a gable.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig05-HippedGableRoof.gif" alt="HippedGableRoof" width="239" height="169" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">GAMBREL_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A ridged roof divided on each
			 side into a shallower slope above a steeper one.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig06-GambrelRoof.gif" alt="GrambrelRoof" width="237" height="178" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">MANSARD_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having on each side a
			 steeper lower part and a shallower upper part.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig07-MansardRoof.gif" alt="MansardRoof" width="234" height="171" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">BARREL_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof or ceiling having a
			 semicylindrical form.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig08-BarrelRoof.gif" alt="BarrelRoof" width="241" height="170" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">RAINBOW_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A gable roof in the form of a
			 broad Gothic arch, with gently sloping convex surfaces.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig09-RainbowRoof.gif" alt="RainbowRoof" width="238" height="200" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">BUTTERFLY_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A roof having two slopes,
			 each descending inward from the eaves.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig10-ButterflyRoof.gif" alt="ButterflyRoof" width="236" height="158" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">PAVILION_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A pyramidal hip roof.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig11-PavilionRoof.gif" alt="PavilionRoof" width="235" height="140" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">DOME_ROOF</td> 
		  <td width="46%" valign="TOP" align="LEFT">A hemispherical hip
			 roof.</td> 
		  <td width="23%" valign="TOP" align="LEFT"><img src="figures/IfcRoofTypeEnum-Fig12-DomeRoof.gif" alt="Dome" width="240" height="140" border="0"></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT"> FREEFORM</td> 
		  <td width="46%" valign="TOP" align="LEFT">Free form roof </td> 
		  <td width="23%" valign="TOP" align="LEFT">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="30%" valign="TOP" align="LEFT">NOTDEFINED</td> 
		  <td width="46%" valign="TOP" align="LEFT">No specification given</td> 
		  <td width="23%" valign="TOP" align="LEFT">&nbsp;</td> 
		</tr> 
	 </table>

> <font size="-1">NOTE: These figures are only shown as
		  illustrations.</font>
>