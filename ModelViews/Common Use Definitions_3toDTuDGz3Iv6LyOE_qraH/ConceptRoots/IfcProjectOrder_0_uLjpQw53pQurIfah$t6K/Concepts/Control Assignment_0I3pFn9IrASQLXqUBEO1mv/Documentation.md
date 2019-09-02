Figure 1 illustrates **IfcProjectOrder** assignment relationships as indicated:

* _IfcActor_ (_IfcRelAssignsToActor_): Organization issuing the order such as an owner or contractor.

The **IfcProjectOrder** may have assignments of its own using the _IfcRelAssignsToControl_ relationship where _RelatingControl_ refers to the **IfcProjectOrder** and _RelatedObjects_ contains one or more objects of the following types:

* _IfcActor_: Organization(s) contracted to fulfill the order, typically a single contractor, subcontractor, or supplier. 

!["Assignment Use Definition"](../../../figures/IfcProjectOrder-Assignment.png "Figure 1 &mdash; Project order assignment")