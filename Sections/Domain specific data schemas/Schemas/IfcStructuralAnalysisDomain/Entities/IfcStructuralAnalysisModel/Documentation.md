﻿The _IfcStructuralAnalysisModel_ is used to assemble all information needed to represent a structural analysis model. It encompasses certain general properties (such as analysis type), references to all contained structural members, structural supports or connections, as well as loads and the respective load results.

Important functionalities for the description of an analysis model are derived from existing IFC entities:

* From _IfcSystem_ it inherits the ability to couple the analysis model via _IfcRelServicesBuildings_ to one or more _IfcBuilding_s as necessary.
* From _IfcGroup_ it inherits the inverse attribute _IsGroupedBy_, pointing to the relationship class _IfcRelAssignsToGroup_. This allows to group structural members (instances of _IfcStructuralMember_), and supports (instances of _IfcStructuralConnection_) which belong to a specific analysis model. 
>> NOTE&nbsp; Loads (as instances of _IfcStructuralAction_) are not included through _IsGroupedBy_. Loads are assigned through the _LoadedBy_ attribute relationship, using load groups as a grouping mechanism. Only top-level load groups should be referenced via _LoadedBy_, i.e. load combinations if any load combinations exist, or load cases if no load combinations exist in this analysis model. 
>> NOTE&nbsp; Results (as instances of _IfcStructuralReaction_) are not included through _IsGroupedBy_. Results are assigned through the _HasResults_ attribute relationship, using result groups as a grouping mechanism. 
* From _IfcObject_ it inherits the inverse attribute _IsDecomposedBy_ pointing to the relationship class _IfcRelNests_. It provides the hierarchy between the separate (partial) analysis models.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Attribute _SharedPlacement_ and informal propositions added, allowing for easy retrieval of the common object placement and for specification of the analysis model's coordiante system before any structural item is instantiated. WHERE rule added.

{ .spec-head}
Informal Propositions:

1. If one or more structural item (instance of a subtype of _IfcStructuralItem_) is grouped into an _IfcStructuralAnalysisModel_, the attribute _SharedPlacement_ shall be provided with a value.
2. The _ObjectPlacement_s of all structural items which are grouped into the same instance of _IfcStructuralAnalysisModel_ shall refer to the same instance of _IfcObjectPlacement_ as _IfcStructuralAnalysisModel.SharedPlacement_.

> NOTE&nbsp; This rule is necessary to achieve consistent topology representations. The topology representations of structural items in an analysis model are meant to share vertices and edges und must therefore have the same object placement.

> NOTE&nbsp; A structural item may be grouped into more than one analysis model. In this case, all these models must use the same instance of _IfcObjectPlacement_.
