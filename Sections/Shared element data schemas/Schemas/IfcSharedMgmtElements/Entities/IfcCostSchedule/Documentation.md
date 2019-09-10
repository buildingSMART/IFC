An _IfcCostSchedule_ brings together instances of _IfcCostItem_ either for the purpose of identifying purely cost information as in an estimate for constructions costs or for including cost information within another presentation form such as a work order.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Attribute _ID_ renamed to _Identification_ and promoted to supertype _IfcControl_, _PredefinedType_ made optional, attributes _PreparedBy_, _SubmittedBy_, _TargetUsers_ removed.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifccostschedule.htm)

{ .use-head}
Object Approval

The [Object Approval](../../templates/object-approval.htm) concept applies to this entity.

Approvals may be associated to indicate the status of acceptance or rejection using the [IfcRelAssociatesApproval](../../ifccontrolextension/lexical/ifcrelassociatesapproval.htm) relationship where _RelatingApproval_ refers to an [IfcApproval](../../ifcapprovalresource/lexical/ifcapproval.htm) and _RelatedObjects_ contains the **IfcCostSchedule**. Approvals may be split into sub-approvals using [IfcApprovalRelationship](../../ifcapprovalresource/lexical/ifcapprovalrelationship.htm) to track approval status separately for each party where _RelatingApproval_ refers to the higher-level approval and _RelatedApprovals_ contains one or more lower-level approvals. The hierarchy of approvals implies sequencing such that a higher-level approval is not executed until all of its lower-level approvals have been accepted.

  
  
{ .use-head}
Control Assignment

The [Control Assignment](../../templates/control-assignment.htm) concept applies to this entity.

The **IfcCostSchedule** may be assigned to the following entities using relationships as indicated:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm) ([IfcRelAssignsToActor](../../ifckernel/lexical/ifcrelassignstoactor.htm)): Persons and organizations involved in the preparation, submittal, and as target users.

The **IfcCostSchedule** may have assignments of its own using the [IfcRelAssignsToControl](../../ifckernel/lexical/ifcrelassignstocontrol.htm) relationship where _RelatingControl_ refers to the **IfcCostSchedule** and _RelatedObjects_ contains one or more objects of the following types:

* [IfcCostItem](../../ifcsharedmgmtelements/lexical/ifccostitem.htm): Indicates costs published within this cost schedule, typically a single root cost item forming a hierarchy of nested cost items.
