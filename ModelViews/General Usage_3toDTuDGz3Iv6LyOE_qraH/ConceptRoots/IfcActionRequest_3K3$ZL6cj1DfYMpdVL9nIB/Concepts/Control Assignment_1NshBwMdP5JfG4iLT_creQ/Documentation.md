As shown in Figure 1, an **IfcActionRequest** may be assigned to the following entities using relationships as indicated:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm) ([IfcRelAssignsToActor](../../ifckernel/lexical/ifcrelassignstoactor.htm)): Person or organization issuing the request such as a tenant or owner.

The **IfcActionRequest** may have assignments of its own using the [IfcRelAssignsToControl](../../ifckernel/lexical/ifcrelassignstocontrol.htm) relationship where _RelatingControl_ refers to the **IfcActionRequest** and _RelatedObjects_ contains one or more objects of the following types:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm): Person or organization(s) fulfilling the request such as a facilities manager or contractor. 

!["Assignment Use Definition"](../../../figures/ifcactionrequest-assignment.png "Figure 1 &mdash; Action request assignment")