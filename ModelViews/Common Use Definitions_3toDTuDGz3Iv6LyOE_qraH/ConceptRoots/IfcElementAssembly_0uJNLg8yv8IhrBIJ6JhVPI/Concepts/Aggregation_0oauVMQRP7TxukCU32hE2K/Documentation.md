The _IfcElementAssembly_ shall represent an aggregate, i.e. it should have other elements, being subtypes of _IfcElement_, as contained (sub)parts. The table above only represents a selection of subtypes of _IfcElement_ that are legitimate as parts in an _IfcElementAssembly_

* The _IfcElementAssembly_ is an aggregate i.e. being composed by other elements and acting as an assembly using the objectified relationship _IfcRelAggregates_, refering to it by its inverse attribute _SELF\IfcObjectDefinition.IsDecomposedBy_. Components of an assembly are described by instances of subtypes of _IfcElement_.
* In this case, the contained subtypes of _IfcElement_ shall not be additionally contained in the project spatial hierarchy, i.e. the inverse attribute _SELF\IfcElement.ContainedInStructure_ of those _IfcElement_'s shall be _NIL._

Figure 1 illustrates spatial containment and element aggregation relationships.

!["containment relationships"](../../../figures/IfcElementAssembly-Containment.png "Figure 1 &mdash; Element assembly containment")