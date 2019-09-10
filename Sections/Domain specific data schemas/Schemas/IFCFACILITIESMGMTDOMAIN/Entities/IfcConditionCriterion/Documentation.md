An _IfcConditionCriterion_ is a particular measured or assessed criterion that contributes to the overall condition of an artifact.

> <font color="#0000FF" size="-1">HISTORY: New class in IFC 2x2 </font>

### Use Definitions
An _IfcConditionCriterion_ may be either an observed/assessed value or a measured value. This is determined by selection through the _IfcConditionCriterionSelect_ type that has a datatype either of _IfcLabel_ (for a numeric or alphanumeric scale observation e.g. on a scale of 1 to 10 where 1 represents 'as new' and 10 represents 'urgent replacement required') or of _IfcMeasureWithUnit_ (for a measured criterion that also includes units of measure).

Each criterion must be named and optionally, may also have a description. A description used for a condition should be persistent so that there is absolute consistency in condition recording.
