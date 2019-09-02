A goniometric light gets its intensity distribution function (how much light goes in any one direction) from one of two sources: (i) an industry-standard file, (ii) from distribution data passed directly via the _IfcLightIntensityDistribution_.

The light distribution provides the luminous intensity distribution according to some standardized light distribution curves.

SELECT

<table> 
		<tr> 
		  <td><em>Type</em></td> 
		  <td><em>Definition</em></td> 
		</tr> 
		<tr> 
		  <td valign="top"><em>IfcExternalReference</em></td> 
		  <td valign="top">Light distribution is represented by a standard photometric data file such as Eulumdat, IES, CIBSE TM14. </td> 
		</tr> 
		<tr> 
		  <td valign="top"><em>IfcLightIntensityDistribution</em></td> 
		  <td valign="top">For representing a light distribution directly the
			 following values needs to be given in a table like structure with column and
			 row headings. These headings should contain the angles (C/&#947; or B/&#946; )
			 and the table body contains the intensity values, (normally normalized to
			 cd/Klm). The angles can be non- equidistant and the angle steps can be almost
			 any value in the valid range, so a list of all available angles in both
			 directions covers all cases. </td> 
		</tr> 
	 </table>

> HISTORY&nbsp; New type in IFC2x2.