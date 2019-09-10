An _IfcProjectOrder_ sets common properties for project orders issued in a construction or facilities management project.

> <font color="#0000ff" size="-1">HISTORY:
New Entity in IFC Release 2.0. Modified in IFC 2x2</font>

****Use Definitions****

Actor attributes such as the organization to which the order is sent, issuing organization, person responsible atc. are handled by assigning instances of _IfcActor_ through _IfcRelAssignsToProjectOrder_. The _IfcActorRole_ must be asserted with the value of the role set when used in this context.

A work plan (acting as a service) may be assigned to a project order (acting as a client) to describe how the project order should be fulfilled. This is handled by assigning instances of _IfcWorkPlan_ through _IfcRelAssignsToProjectOrder_.

The reverse of this situation may be true whereby the work plan (acting as a client) may have project orders (acting as a service). This is handled by assigning instances of _IfcProjectOrder_ to an _IfcWorkPlan_ through _IfcRelAssignsToControl_.

Approvals including signoff, authorization etc. are handled using the the _IfcRelAssociatesApproval_ relationship class.

A cost schedule may be assigned to a project order are handled through the _IfcRelAssignsToProjectOrder_ relationship.

****Property Set Use Definition****:

The property sets relating to an _IfcProjectOrder_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcProjectOrder_ are part of this IFC release:

* [Pset_ProjectOrderChangeOrder](../../psd/IfcSharedMgmtElements/Pset_ProjectOrderChangeOrder.xml): specific property set for the properties of a change order, if available
* [Pset_ProjectOrderMaintenanceWorkOrder](../../psd/IfcSharedMgmtElements/Pset_ProjectOrderMaintenanceWorkOrder.xml): specific property set for the properties of a maintenance work order, if available 
* [Pset_ProjectOrderMoveOrder](../../psd/IfcSharedMgmtElements/Pset_ProjectOrderMoveOrder.xml): specific property set for the properties of a move order, if available 
* [Pset_ProjectOrderPurchaseOrder](../../psd/IfcSharedMgmtElements/Pset_ProjectOrderPurchaseOrder.xml): specific property set for the properties of a purchase order, if available 
* [Pset_ProjectOrderWorkOrder](../../psd/IfcSharedMgmtElements/Pset_ProjectOrderWorkOrder.xml): specific property set for the properties of a general work order, if available
