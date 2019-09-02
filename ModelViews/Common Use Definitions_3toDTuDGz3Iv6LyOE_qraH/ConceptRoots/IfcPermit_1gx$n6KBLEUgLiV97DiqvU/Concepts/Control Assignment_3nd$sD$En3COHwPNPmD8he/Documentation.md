Figure 1 illustrates assignment relationships as indicated:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm) ([IfcRelAssignsToActor](../../ifckernel/lexical/ifcrelassignstoactor.htm)): Organization issuing the permit such as a local government agency or security organization.

The **IfcPermit** may have assignments of its own using the [IfcRelAssignsToControl](../../ifckernel/lexical/ifcrelassignstocontrol.htm) relationship where _RelatingControl_ refers to the **IfcPermit** and _RelatedObjects_ contains one or more objects of the following types:

* [IfcActor](../../ifckernel/lexical/ifcactor.htm): Organization(s) bound to the permit, typically a single contractor. 

!["Assignment Use Definition"](../../../figures/IfcPermit-Assignment.png "Figure 1 &mdash; Permit assignment")