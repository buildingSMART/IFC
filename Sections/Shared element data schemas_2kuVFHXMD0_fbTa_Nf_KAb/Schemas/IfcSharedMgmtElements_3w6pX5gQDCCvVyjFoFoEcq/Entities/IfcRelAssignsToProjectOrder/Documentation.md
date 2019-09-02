An _IfcRelAssignsToProjectOrder_ is a relationship class that captures the incidence of a project order for a set of objects and whose occurrences can be recorded within a project record in sequence as a series of events.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x2</font>

### Use Definitions
_IfcRelAssignsToProjectOrder_ is a subtype of _IfcRelAssignsToControl_. It acts so as to assign items to a project order. The instance of _IfcProjectOrder_ acts as the relating control (which is inherited from _IfcRelAssignsToControl_).

Specific objects may be assigned to the project order via the inherited _IfcRelAssignsToControl.RelatedObjects_ attribute. Examples are a cost schedule (_IfcCostSchedule_), a work plan (_IfcWorkPlan_), actors concerned with the project order (_IfcActor_) etc.

It may also be relevant to assign physical components to the order to identify that this is the originating order for such objects. This can be particularly relevant in the operating phase of the facility lifecycle where the Facilities Manager may wish to obtain details about the original purchase of components. It is more efficient to achieve this through assigning the objects to the project order through _IfcRelAssignsToProjectOrder_ rather than assigning the project order to each object through multiple instances of _IfcRelAssignsToProduct_.