_IfcRelFillsElement_ is an objectified relationship between an opening element and an element that fills (or partially fills) the opening element. It is an one-to-one relationship.

> NOTE&nbsp; View definitions or implementer agreements may restrict an opening to be filled by one filling element only.

As shown in Figure 1, the insertion of a door into a wall is represented by two separate relationships. First the door opening is created within the wall by _IfcWall(StandardCase) &lt;-- IfcRelVoidsElement --&gt; IfcOpeningElement_, then the door is inserted within the opening by _IfcOpeningElement &lt;-- IfcRelFillsElement --&gt; IfcDoor_.

&nbsp;

!["relationships for filling"](../../../figures/ifcrelfillselements-fig1.png "Figure 1 &mdash; Relationships for element filling")

> HISTORY&nbsp; New entity in IFC1.0