An _IfcRelAssociatesAppliedValue_ is a subtype of _IfcRelAssociates_ that enables the association of an instance of IfcAppliedValue with one or more instances of _IfcObject_.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x2.</font>

### Use Definitions
Because IfcRelAssociatesAppliedValue is a subtype of IfcRelAssociates, this means that a single instance of _IfcCostValue_ or _IfcEnvironmentalImpactValue_ can be related to many objects of whatever type (product, process, resource etc.)

Note that _IfcRelAssociatesAppliedValue_, when used for costing purposes, should be used only for relating specific cost values to objects and not for relating cost schedule items to cost schedule (for which purpose _IfcRelSchedulesCostItems_ should be used).