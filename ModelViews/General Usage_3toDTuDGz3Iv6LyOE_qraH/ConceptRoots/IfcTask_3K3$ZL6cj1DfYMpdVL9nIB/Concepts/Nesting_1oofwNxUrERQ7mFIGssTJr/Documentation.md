_IfcTask_ may be contained within an _IfcTask_ using the _IfcRelNests_ relationship. An _IfcTask_ may in turn nest other _IfcTask_, _IfcProcedure_ or _IfcEvent_ entities. Such nesting indicates decomposed level of detail. From IFC4 onwards it is required to have a summary task (root of all tasks), which is used to define a link to the work plan or work schedule. All subtasks of the summary tasks are then implicitly linked to this work plan or work schedule. Please note that the summary task is used for data organization and not meant to store typical task information as defined by the user. It is therefore recommended that the summary task is hidden from the user to avoid confusion. Please also note that _IfcRelNests_ is used to show the dependency between regular tasks and recurring task definitions (please see the section about time and duration use definitions).

As shown in Figure 1, the installation of a number of items of equipment within a particular space may be the subject of a single task which is identified as 'fix equipment in space 123'. _IfcTask_ represents the occurrence of a work performance of a type of process in a construction plan.

!["task example"](../../../figures/ifctask_example.png "Figure 1 &mdash; Task visualization")

A task may nest other tasks as sub-items; the nesting relationship is modeled by _IfcRelNests_ as shown in Figure 2. For example, the construction of a stud wall may be designated as a nesting task named 'install wall #1' including other tasks such as 'install dry wall', 'install studs', 'wall taping', and 'erect wall' as sub-processes. A value that indicates the relative tree view position of the task (in comparison to the tree view position of other tasks and the task hierarchy defined by _IfcRelNests_).

The task order information that is used for viewing purposes is derived from the order defined by the _IfcRelNests_ relationship and thus is independent of the logical task order defined through _IfcRelSequence_. The hierarchy and order defined through _IfcRelNests_ enables to order the tasks in a tree view or list view structure.

!["task instantiation diagram"](../../../figures/ifctask_instantiation_diagram.png "Figure 2 &mdash; Task nesting relationships")

A top-level task is declared within the _IfcProject_ using the _IfcRelDeclares_ relationship.