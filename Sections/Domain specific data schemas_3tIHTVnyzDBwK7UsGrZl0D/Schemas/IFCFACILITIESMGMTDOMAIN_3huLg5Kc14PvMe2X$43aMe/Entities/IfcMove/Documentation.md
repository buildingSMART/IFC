An _IfcMove_ is an activity that moves people, groups within an organization or complete organizations together with their associated furniture and equipment from one place to another. The objects to be moved, normally people, equipment, and furniture, are assigned by the _IfcRelAssignsToProcess_ relationship.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0<br>PunchList attribute datatype changed from IfcLabel to
		IfcText<br></font>

### Use Definitions
Actors, equipment and furniture are moved from one IfcSpatialStructureElement to another. The IfcSpatialStructureElement to be moved from and that to be moved to are assigned to the IfcMove class using the IfcRelAssignsToProcess relationship.

The actors (as _IfcActor_), equipment and furnitures to be moved are assigned to the _IfcMove_ using the _IfcRelAssignsToProcess_ relationship

Each _IfcMove_ must have a name. This requirement is enforced by a rule.

The inherited attribute _OperatesOn_ refers to the _IfcRelAssignsToProcess_ relationship, keeping the reference to _IfcActor, IfcEquipmentElement_and_IfcFurnishingElement_. The _QuantityInProcess_ attribute at the relationship object can be used to specify a quantity of the objects to be moved.

Constraints may be applied to a move through instances of the _IfcConstraint_ class (or its subtypes) that are associated through the _IfcRelAssociatesConstraint_ relationship class

Moves can be nested, i.e. a move object can contain other (more detailed) move objects. This is handled by the _IfcRelNests_ relationship pointing (with RelatingObject) to the containing move and (with RelatedObjects) to the contained (sub)moves.

Moves are assigned to a move schedule (represented as _IfcWorkSchedule_ with Purpose attribute '_Move_') by using the _IfcRelAssignsTask_ relationship.