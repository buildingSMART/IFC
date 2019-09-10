An _IfcPropertyListValue_ defines a property that has several (numeric or descriptive) values assigned, these values are given by an ordered list.

An _IfcPropertyListValue_ is a list of values. The order in which values appear is significant. Each value in the list is unique i.e. no duplicate values are allowed. All list members should be of the same type.

The unit applicable to all values is handled by the _Unit_ attribute:

* If the _Unit_ attribute is not given, then the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _Unit_ attribute is given, then the unit assigned by the _Unit_ attribute overrides the globally assigned unit.

Example of a property with list value is:

<table cellpadding="2" cellspacing="2" border="1" width="600"> 
		<tr valign="TOP"> 
		  <td valign="TOP" width="15%"><b>Name</b></td> 
		  <td valign="TOP" width="30%"><b>ListValues</b></td> 
		  <td valign="TOP" width="25%"><b>Type <br></b><font size="-1">(through
			 IfcValue)</font></td> 
		  <td valign="TOP" width="30%"><b>Unit <br></b></td> 
		</tr> 
		<tr> 
		  <td width="15%">ApplicableSizes</td> 
		  <td width="30%">1200</td> 
		  <td width="25%"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%">-</td> 
		</tr> 
		<tr> 
		  <td width="15%">-</td> 
		  <td width="30%">1600</td> 
		  <td width="25%"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%">-</td> 
		</tr> 
		<tr> 
		  <td width="15%">-</td> 
		  <td width="30%">2400</td> 
		  <td width="25%"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%">-</td> 
		</tr> 
	 </table>

> <font color="#0000FF" size="-1">HISTORY: New Entity in Release IFC 2x
		  Edition 2.</font>
>