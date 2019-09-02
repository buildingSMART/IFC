A property with a range value (_IfcPropertyTableValue_) defines a property object which has two lists of (numeric or descriptive) values assigned, the values specifying a table with two columns. The defining values provide the first column and establish the scope for the defined values (the second column). Interpolations are out of scope of the _IfcPropertyTableValue_. An optional _Expression_ attribute may give the equation used for deriving the range value, which is for information purposes only.

The _IfcPropertyTableValue_ defines a defining/defined property value combination for which the property name, the table with defining and defined values with measure type (and optional the units for defining and defined values)are given.

The units are handled by the _DefiningUnit_ and _DefinedUnit_ attributes:

* If the _DefiningUnit_ or _DefinedUnit_ attribute is not given, then the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _DefiningUnit_ or _DefinedUnit_ attribute is given, then the unit assigned by the unit attribute overrides the globally assigned unit.

The _IfcPropertyTableValue_ allows for the specification of a table of defining/defined value pairs of the property description.

Examples of a property with range value are:

<table cellpadding="2" cellspacing="2" border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" width="15%"><b>Name</b></td> 
		  <td valign="TOP" align="LEFT" width="10%"><b>DefiningValues</b></td> 
		  <td valign="TOP" align="LEFT" width="15%"><b>DefiningValue Type
			 <br></b>(through IfcValue)</td> 
		  <td valign="TOP" align="LEFT" width="10%"><b>DefinedValues</b></td> 
		  <td valign="TOP" align="LEFT" width="15%"><b>DefinedValue Type
			 <br></b>(through <i>IfcValue</i>)</td> 
		  <td valign="TOP" align="LEFT" width="15%"><b>DefingUnit </b></td> 
		  <td valign="TOP" align="LEFT" width="15%"><b>DefinedUnit</b></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" align="LEFT">SoundTransmissionLoss</td> 
		  <td>100</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>20</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td>- </td> 
		  <td>dB</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" bgcolor="#C8C8C8">&nbsp;</td> 
		  <td>200</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>42</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" bgcolor="#C8C8C8">&nbsp;</td> 
		  <td>400</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>46</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" bgcolor="#C8C8C8">&nbsp;</td> 
		  <td>800</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>56</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" bgcolor="#C8C8C8">&nbsp;</td> 
		  <td>1600</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>60</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td valign="TOP" align="LEFT" bgcolor="#C8C8C8">&nbsp;</td> 
		  <td>3200</td> 
		  <td><i>IfcFrequencyMeasure</i></td> 
		  <td>65</td> 
		  <td><i>IfcNumericMeasure</i></td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		  <td bgcolor="#C8C8C8">&nbsp;</td> 
		</tr> 
	 </table>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 2x.
		  </font>
>

Informal propositions:

1. The list of _DerivedValues_ and the list of _DefiningValues_ are corresponding lists.