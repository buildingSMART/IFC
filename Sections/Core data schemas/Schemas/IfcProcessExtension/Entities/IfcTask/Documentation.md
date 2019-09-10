An _IfcTask_ is an identifiable unit of work to be carried out independently of any other units of work in a construction project.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
		Release 1.0. Renamed from IfcWorkTask in IFC 2x.</font>

**Use Definitions**

Work is identified as tasks (i.e. _IfcTask_) that are capable of either containing other tasks or being sub-items of other tasks. A task can be used to describe a process for the construction or installation of products.

Each instance of _IfcTask_ is given a name that is indicative of its content. A textual description of the the task may be be provided.

Instances of _IfcTask_ may be assigned to an _IfcWorkControl_ (either a work plan or a work schedule) through the _IfcRelAssignsTasks_ relationship class.

The installation of a number of items of equipment within a particular space may be the subject of a single task which is identified as e.g. &#145;fix equipment in space 123&#146;. _IfcTask_ represents the occurrence of a work performance of a type of process in a construction plan.

A task can nest other tasks as sub-items; the nesting relationship is modeled by _IfcRelNests_. For example, the construction of a stud wall may be designated as a nesting task named &#145;install wall #1&#146; including other tasks such as &#145;install dry wall&#146;, &#145;install studs&#146;, &#145;wall taping&#146;, and &#145;erect wall&#146; as sub-processes.

Special information relating to a task is asserted using _IfcTask.ObjectType_ (inherited from _IfcObject_). Examples that may be used include fixed duration, fixed unit, fixed work.

The sequential relationships between tasks are represented by _IfcRelSequence_ in _IfcKernel_ schema.

Resource used by tasks are assigned by _IfcRelAssignsToProcess_. Quantities of resources consumed by the task are dealt with by defining the _IfcElementQuantity_ for the resource and not at the instance of _IfcTask_.

An _IfcTask_ may be assigned a Work Breakdown Structure (WBS) code. A WBS code is dealt with as a classification of task and is associated to a task occurrence using the _IfcRelAssociatesClassification_ relationship class. As well as being to designate the code, the classification structure of the IFC model also enables the source of the work breakdown structure classification to be identified.
