The _IfcAppliedValueSelect_ defines the selection of whether a value (expressed as a ratio) or an amount should be used as the value for an _IfcAppliedValue_.

**Select from:**

* IfcMeasureWithUnit
* IfcMonetaryMeasure
* IfcRatioMeasure

> <font size="-1" color="#0000FF">HISTORY: New SELECT type in IFC
		2x2.</font>

**Use Definitions**

Selecting _IfcMeasureWithUnit_ allows the specification of both the actual figure for the value together with the currency (for a cost value) or an environmental measurement unit (in the case of an environmental impact value) in which the value is represented.

Selecting _IfcMonetaryMeasure_ allows the specification only of the value, the currency being as set by the global context

Selecting _IfcRatioMeasure_ assumes that the amount is a percentage or other REAL number. Note that if the amount is normally specified as -20%, then this figure will need to be converted to a multiplier of 0.8
