A property with a single value (_IfcPropertySingleValue_) defines a property object which has a single (numeric or descriptive) value assigned. It defines a property - single value combination for which the property name, the value with measure type (and optionally the unit) is given.

The unit is handled by the _Unit_ attribute:

* If the _Unit_ attribute is not given, then the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _Unit_ attribute is given, then the unit assigned by the _Unit_ attribute overrides the globally assigned unit.

Examples of a property with single value are:

<table cellpadding="2" cellspacing="2" border="1"> 
		<tr valign="TOP"> 
		  <td valign="TOP" width="15%"><b>Name</b></td> 
		  <td valign="TOP" width="30%"><b>NominalValue</b></td> 
		  <td valign="TOP" width="25%"><b>Type <br></b><font size="-1">(through
			 <i>IfcValue</i>)</font></td> 
		  <td valign="TOP" width="30%"><b>Unit <br></b></td> 
		</tr> 
		<tr> 
		  <td width="15%">Description</td> 
		  <td width="30%">Manufacturer "A" door</td> 
		  <td width="25%"><i>IfcLabel</i></td> 
		  <td width="30%">-</td> 
		</tr> 
		<tr> 
		  <td width="15%">PanelThickness</td> 
		  <td width="30%">0.12</td> 
		  <td width="25%"><i>IfcPositiveLengthMeasure</i></td> 
		  <td width="30%">- </td> 
		</tr> 
		<tr> 
		  <td width="15%">ThermalTransmittance</td> 
		  <td width="30%">2.6</td> 
		  <td width="25%"><i>IfcThermalTransmittanceMeasure</i></td> 
		  <td width="30%">W/(m<sup>2</sup>K)</td> 
		</tr> 
	 </table>

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.0. The entity has been renamed from IfcSimpleProperty in IFC Release
		  2x</font>
>