An _IfcAppliedValue_ is an abstract supertype that specifies the common attributes for cost and environmental values that may be applied to objects within the IFC model.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2x2</font>

**Use Definitions**

The extent of the _IfcAppliedValue_ is determined by the _AppliedValue_ attribute which may be defined either as an _IfcMeasureWithUnit_ or as an _IfcMonetaryMeasure_ or as an _IfcRatioMeasure_ via the _IfcAppliedValueSelect_ type.

Optionally, an _IfcAppliedValue_ may have an applicable date. This is intended to fix the date on which the value became relevant for use. It may be the date on which the value was set in the model or it may be a prior or future date when the value becomes operable. It should be noted that the datatype for _IfcAppliedValue.ApplicableDate_ is _IfcDateTimeSelect_. This enables either a calendar date or a date and time to be selected. The option of selecting a time only without a date is also possible through this select mechanism but should not be used in the case of an applied value.

Similarly, an _IfcAppliedValue_ may have a 'fixed until' date. This is intended to fix the date on which the value ceases to be relevant for use.

An instance of _IfcAppliedValue_ may have a unit basis asserted. This is defined as an _IfcMeasureWithUnit_ that determines the extent of the unit value for application purposes. It is assumed that when this attribute is asserted, then the value given to _IfcAppliedValue_ is that for unit quantity. This is not enforced within the IFC schema and thus needs to be controlled within an application.