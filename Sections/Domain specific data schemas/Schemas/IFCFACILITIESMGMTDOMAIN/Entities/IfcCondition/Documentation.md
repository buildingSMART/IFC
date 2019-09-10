An _IfcCondition_ determines the state or condition of an element at a particular point in time

> <font color="#0000FF" size="-1">HISTORY: New class in IFC
		2x2</font>

### Use Definitions
_IfcCondition_ is a particular subtype of _IfcGroup_ that can contain only instances of _IfcConditionCriterion_. The objectified relationship class _IfcRelAssignsToGroup_ is used to assign the related instances of _IfcConditionCriterion_ to the relating instance of _IfcCondition_.

An _IfcCondition_ is determined either from an observed or a measured state (see _IfcConditionCriterion_). The condition is determined at a particular point in time, the time being determined through the _IfcRelAssociatesDateTime_ class with an appropriate designation for the value of the DateTimeType e.g. AssessmentDate. Note that other dates may be assigned to _IfcCondition_ for relevant purposes e.g. to recommend the date for the next condition assessment.

_IfcRelAssignsToProduct_ is used to relate one or more instances of _IfcCondition_ to an artifact that is an instance of a subtype of _IfcProduct_. For an instance of _IfcAsset_, condition is related through the use of _IfcRelAssignsToGroup_.