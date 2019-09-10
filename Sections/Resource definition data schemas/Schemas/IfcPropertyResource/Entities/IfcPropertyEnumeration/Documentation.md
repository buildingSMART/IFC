A collection of simple or measure values that define a prescribed set of alternatives from which 'enumeration values' are selected. This enables inclusion of enumeration values in property sets. _IfcPropertyEnumeration_ provides a name for the enumeration as well as a list of unique (numeric or descriptive) values (that may have a measure type assigned). The entity defines the list of potential enumerators to be exchanged together (or separately) with properties of type _IfcPropertyEnumeratedValue_ that selects their actual property values from this enumeration.

The unit is handled by the _Unit_ attribute:

* If the _Unit_ attribute is not given, than the unit is already implied by the type of _IfcMeasureValue_ or _IfcDerivedMeasureValue_. The associated unit can be found at the _IfcUnitAssignment_ globally defined at the project level (_IfcProject.UnitsInContext_).
*  If the _Unit_ attribute is given, the unit assigned by the unit attribute overrides the globally assigned unit.

<table border="1" cellpadding="2" cellspacing="2" width="80%">
  <tbody>
    <tr>
      <td width="30%"><b>Name</b></td>
      <td width="30%"><b>EnumerationValues</b></td>
      <td width="25%"><b>Type </b><font size="-1">(through <i>IfcValue</i>)</font></td>
      <td width="15%"><b>Unit</b></td>
    </tr>
    <tr>
      <td>PEnum_DamperBladeAction</td>
      <td>Parallel</td>
      <td><i>IfcString</i></td>
      <td>-</td>
    </tr>
    <tr>
      <td>&nbsp;</td>
      <td>Opposed</td>
      <td><i>IfcString</i></td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>&nbsp;</td>
      <td>Other</td>
      <td><i>IfcString</i></td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>&nbsp;</td>
      <td>Unset</td>
      <td><i>IfcString</i></td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">
HISTORY: New Entity in IFC Release 2.0, capabilities enhanced in IFC
Release 2x. Entity has been renamed from IfcEnumeration in IFC Release
2x.</font>
>
