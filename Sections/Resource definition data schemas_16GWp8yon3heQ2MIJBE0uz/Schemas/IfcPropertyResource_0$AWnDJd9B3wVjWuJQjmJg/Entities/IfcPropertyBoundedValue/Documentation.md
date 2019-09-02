A property with a bounded value (_IfcPropertyBoundedValue_) defines a property object which has a maximum of two (numeric or descriptive) values assigned, the first value specifying the upper bound and the second value specifying the lower bound. It defines a property - value bound (min-max) combination for which the property name, the upper bound value with measure type, the lower bound value with measure type (and optional the unit) is given.

The unit is handled by the _Unit_ attribute:

* If the _Unit_ attribute is not given, then the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _Unit_ attribute is given, then the unit assigned by the _Unit_ attribute overrides the globally assigned unit.

The _IfcPropertyBoundedValue_ allows for the specification of an interval for the value component of the property description. <font color="#0000FF">If either the <i>LowerBoundValue</i> or the
		<i>UpperBoundValue</i> is not given, then it indicates an open bound (either a
		minimum value or a maximum value). The interval is by definition inclusive,
		i.e. the value given for the <i>LowerBoundValue</i> or the
		<i>UpperBoundValue</i> is included in the interval.</font>

Examples of a property with bounded value are:

<table border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP" width="15%"><b>Name</b></td> 
		  <td valign="TOP" width="15%"><b>UpperBoundValue</b></td> 
		  <td valign="TOP" width="15%"><b>LowerBoundValue</b></td> 
		  <td valign="TOP" width="25%"><b>Type <br></b><font size="-1">(through
			 <i>IfcValue</i>, WR1 ensures same type for both values)</font></td> 
		  <td valign="TOP" width="30%"><b>Unit <br></b></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="15%" valign="TOP" align="LEFT">OverallHeight</td> 
		  <td width="30%" valign="TOP" align="LEFT">1930</td> 
		  <td width="25%" valign="TOP" align="LEFT">2300</td> 
		  <td width="25%" valign="TOP" align="LEFT"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%" valign="TOP" align="LEFT">- </td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="15%" valign="TOP" align="LEFT">OverallWidth</td> 
		  <td width="30%" valign="TOP" align="LEFT">0.9</td> 
		  <td width="25%" valign="TOP" align="LEFT">1.25</td> 
		  <td width="25%" valign="TOP" align="LEFT"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%" valign="TOP" align="LEFT">m</td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="15%" valign="TOP" align="LEFT"><font color="#0000FF">MaxHeight</font></td> 
		  <td width="30%" valign="TOP" align="LEFT"><font color="#0000FF">20.0</font></td> 
		  <td width="25%" valign="TOP" align="LEFT"><font color="#0000FF">&lt;nil&gt;</font></td> 
		  <td width="25%" valign="TOP" align="LEFT"><font color="#0000FF"><i>IfcPositiveLengthMeasure</i></font></td> 
		  <td width="30%" valign="TOP" align="LEFT"><font color="#0000FF">-</font></td> 
		</tr> 
		<tr valign="TOP"> 
		  <td width="15%" valign="TOP" align="LEFT"><font color="#0000FF">MinWeight</font></td> 
		  <td width="30%" valign="TOP" align="LEFT"><font color="#0000FF">&lt;nil&gt;</font></td> 
		  <td width="25%" valign="TOP" align="LEFT"><font color="#0000FF">20</font></td> 
		  <td width="25%" valign="TOP" align="LEFT"><font color="#0000FF"><i>IfcMassMeasure</i></font></td> 
		  <td width="30%" valign="TOP" align="LEFT"><font color="#0000FF">kg</font></td> 
		</tr> 
	 </table>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 2x.
		  </font>
> 


> <font color="#FF0000" size="-1">IFC2x PLATFORM CHANGE: The
		attribute type of the attribute <i>UpperBoundValue</i> and
		<i>LowerBoundValue</i> has been changed from mandatory to optional with upward
		compatibility for file based exchange.</font>

Informal proposition:

1. If the measure type for the upper and lover bound value is a numeric measure, then the following shall be true: _UpperBoundValue_ &gt; _LowerBoundValue_.