An _IfcProcedure_ is an identifiable step to be taken within a process that is considered to occur over zero or a non-measurable period of time.

> <font color="#0000FF" size="-1">HISTORY:New entity in IFC
		2x2</font>

**Use Definitions**

An instance of _IfcProcedure_ may nest other instances of _IfcProcedure_ using _IfcRelNests_. Instances of _IfcProcedure_, since they are subtypes of _IfcProcess_, may also participate in sequence relationships using _IfcRelSequences_.

_IfcProcedure_ is used to capture information about stepped processes such as calibration, start/stop procedures for equipment items etc.

Note that a particular type of _IfcProcedure_ is a caution, warning or other form of advisory note. Typically, it is anticipated that such a procedure would be assigned to the specific _IfcProcess_ for which it gives advice using _IfcRelAssignsToProcess_.

Note that both nesting and sequencing can be supported concurrently. For example, B, C and D may be procedures nested in procedure A. Sequence relationships can also be established such that B precedes C and C precedes D.
