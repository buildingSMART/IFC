﻿_IfcRelSequence_ is a sequential relationship between processes where one process must occur before the other in time and where the timing of the relationship may be described as a type of sequence. The relating process (_IfcRelSequence.RelatingProcess_) is considered to be the predecessor in the relationship (has precedence) whilst the related process (_IfcRelSequence.RelatedProcess_) is the successor.

_IfcRelSequence_ is defined as one-to-one relationship; therefore it assigns one predecessor to one successor.

> HISTORY&nbsp; New entity in IFC1.0.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Relocated to _IfcProcessExtension_ schema. _TimeLag_ and _SequenceType_ made optional. USERDEFINED added to the _IfcSequenceType_ enumeration. _UserDefinedSequenceType_ attribute added. WHERE rule controlling use of the USERDEFINED enumeration added.

{ .use-head}
Use definitions

_IfcRelSequence_ is used to describe the logical sequence relationship that exists between two processes. This logical relationship identifies that there is a predecessor or relating process and a successor or related process. In IFC, there may be one predecessor and one successor in the relationship. Many occurrences of _IfcRelSequence_ may exist to describe the sequence relationships of a predecessor task with many successor tasks or of many predecessor tasks with one successor task, thus enabling a m:n sequence relationship between tasks. Please note that sequence relationships can be used to define dependencies between process occurrences but also between process types (for further information see _IfcRelDefinesByObject_ and _IfcTaskType_). In case of defining dependencies between process occurrences sequence relationships should stay within the limits of a directed, non-cyclic graph.

A sequence type may be set for a sequence. For tasks assigned to a work schedule, it is expected that the sequence type will be asserted. For a process map, where the sequence relationship between processes is simply a logical flow, it need not be asserted.

A time lag may be assigned to a sequence, and the sequence type defines the way in which the time lag applies to the sequence either as a ratio or percentage of time duration (e.g. start successor task when predecessor is 50% complete) or as a time measure (e.g. start successor task 1 week after commencement of the predecessor task). Care should be used when assigning a time lag to a sequence depending on the setting of the sequence type since there is no checking that the time lag value is in keeping with the sequence type set.
