The **IfcCostSchedule** may be assigned to the following entities using relationships as indicated:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm) ([IfcRelAssignsToActor](../../ifckernel/lexical/ifcrelassignstoactor.htm)): Persons and organizations involved in the preparation, submittal, and as target users.

The **IfcCostSchedule** may have assignments of its own using the [IfcRelAssignsToControl](../../ifckernel/lexical/ifcrelassignstocontrol.htm) relationship where _RelatingControl_ refers to the **IfcCostSchedule** and _RelatedObjects_ contains one or more objects of the following types:

* [IfcCostItem](../../ifcsharedmgmtelements/lexical/ifccostitem.htm): Indicates costs published within this cost schedule, typically a single root cost item forming a hierarchy of nested cost items.