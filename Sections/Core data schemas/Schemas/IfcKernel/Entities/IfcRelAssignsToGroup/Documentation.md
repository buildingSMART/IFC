This objectified relationship (_IfcRelAssignsToGroup_) handles the assignment of objects (subtypes of _IfcObject_) to a group (subtypes of _IfcGroup_).

The relationship handles the assignment of group members to the group object. It allows for grouping arbitrary objects within a group, including other groups. The grouping relationship can be applied in a recursive manner. The resulting group is of type _IfcGroup_. The _Purpose_ attribute defined at the supertype IfcReleationship, may assign a descriptor, that defines the purpose of the group.

The inherited attribute _RelatedObjects_ gives the references to the objects, which are the elements within the group. The _RelatingGroup_ is the group, that comprises all elements.

**Informal proposition**:

1. The group assignment relationship shall be a-cyclic, i.e. a group should not participate in its own grouping relationship.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC Release 1.0.
		  Has been renamed from IfcRelGroups in IFC Release 2x.</font>.
>
