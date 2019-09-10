A property with an enumerated value (_IfcPropertyEnumeratedValue_) defines a property object which has a value assigned which is chosen from an enumeration. It defines a property - value combination for which the property name, the value with measure type (and optional the unit) are given.

> <font size="-1">NOTE: Multiple choices from the property enumeration
		  are supported.</font>
>

The unit is handled by the _Unit_ attribute of the _IfcPropertyEnumeration_:

* If the _Unit_ attribute is not given, then the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _Unit_ attribute is given, then the unit assigned by the unit attribute overrides the globally assigned unit.

More precisely: The _IfcPropertyEnumeratedValue_ defines a property, which value is selected from a defined list of enumerators. The enumerators are stored in a dynamic enumeration of values including the type information from _IfcValue_ (see _IfcPropertyEnumeration_). This enables applications to use an enumeration value as a property within a property set (_IfcPropertySet_) including the allowed list of values. Examples of a property with enumerated value with are:

<table cellpadding="2" cellspacing="2" border="1" width="600"> 
		<tr valign="TOP"> 
		  <td valign="TOP" width="15%"><b>Name&nbsp;</b></td> 
		  <td valign="TOP" width="30%"><b>Value<br></b><font size="-1">(EnumerationValue)</font></td> 
		  <td valign="TOP"><b>Type <br></b><font size="-1">(through
			 IfcValue)</font></td> 
		  <td valign="TOP">ref.<b> IfcPropertyEnumeration<br></b><font size="-1">(Name)</font>&nbsp;</td> 
		</tr> 
		<tr> 
		  <td>BladeAction</td> 
		  <td>Opposed</td> 
		  <td width="25%"><i>IfcString</i></td> 
		  <td width="30%">DamperBladeActionEnum</td> 
		</tr> 
		<tr> 
		  <td>BladeAction</td> 
		  <td>Parallel</td> 
		  <td width="25%"><i>IfcString</i></td> 
		  <td width="30%">DamperBladeActionEnum</td> 
		</tr> 
	 </table>

The _IfcPropertyEnumeratedValue_ refers to an _IfcPropertyEnumeration_, e.g. for the above:

<table cellpadding="2" cellspacing="2" border="1" width="600"> 
		<tr> 
		  <td width="30%"><b>Name</b></td> 
		  <td width="30%"><b>EnumerationValues</b></td> 
		  <td width="25%"><b>Type <br></b><font size="-1">(through
			 IfcValue)</font></td> 
		  <td width="15%"><b>Unit</b></td> 
		</tr> 
		<tr> 
		  <td>DamperBladeActionEnum</td> 
		  <td>(Parallel, Opposed, Other, Unset)</td> 
		  <td><i>IfcString</i></td> 
		  <td>-</td> 
		</tr> 
	 </table>

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC Release
		  2.0, capabilities enhanced in IFC R2x. The entity has been renamed from
		  IfcEnumeratedProperty in IFC Release 2x.</font>
>