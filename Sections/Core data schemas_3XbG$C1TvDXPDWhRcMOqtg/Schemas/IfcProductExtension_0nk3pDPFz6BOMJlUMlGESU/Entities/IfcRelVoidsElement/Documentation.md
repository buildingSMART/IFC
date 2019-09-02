_IfcRelVoidsElement_ is an objectified relationship between a building element and one opening element that creates a void in the element. It is a one-to-one relationship. This relationship implies a Boolean operation of subtraction between the geometric bodies of the element and the opening.

As shown in Figure 1, the insertion of a void into a wall is represented by the relationship _IfcRelVoidsElement_. The opening is created within the wall by _IfcWall(StandardCase) o-- IfcRelVoidsElement --o IfcOpeningElement_.

!["relationships for voiding"](../../../figures/ifcrelvoidselements-fig1.png "Figure 1 &mdash; Relationship for element voiding")

> HISTORY&nbsp; New entity in IFC1.0