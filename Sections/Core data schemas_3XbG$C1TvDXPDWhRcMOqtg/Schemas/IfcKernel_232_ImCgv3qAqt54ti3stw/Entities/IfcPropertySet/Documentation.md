_IfcPropertySet_ defines all dynamically extensible properties. The property set is a container class that holds properties within a property tree. These properties are interpreted according to their name attribute.

The same _IfcPropertySet_ can be assigned to multiple object occurrences; it should then be assigned by a single instance of _IfcRelDefinedByProperties_ to a set of related objects. Those property sets are referred to as shared property sets. It can also be assigned to an object type.

An _IfcPropertySetTemplate_ may define the underlying structure, i.e. the required name, the applicable object or object types to which the property set can be attached, and the individual properties that maybe included.

> NOTE&nbsp; See _IfcRelDefinesByType_ for how to override property sets assigned to an object type within the object occurrence.

> HISTORY&nbsp; New entity in IFC1.0

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; All statically defined property set entities are no longer subtypes of _IfcPropertySet_.

{ .use-head}
Relationship use definition

Property sets are related to other objects by using the relationship object that refers to the corresponding object:

*  **Occurrence Object**: _IfcRelDefinesByProperties_ using the inverse attribute _DefinesOccurrence_. 
*  **Type Object**: using a direct link by inverse attribute _DefinesType_. 
*  **Underlying template**: _IfcRelDefinesByTemplate_ using the inverse attribute _IsDefinedBy_. 
*  **External reference**: subtypes of _IfcRelAssociates_ are used to provide a link to a classification system, or external library providing further reference to the property set. Accessible by inverse attribute _HasAssociations_. 

{ .use-head}
Attribute use definition

Instances of _IfcPropertySet_ are used to assign named sets of individual properties (complex or single properties). Each individual property has a significant name string. Some property sets are included in the IFC specification and have&nbsp;a predefined set of properties indicated by assigning a significant name. These property sets are listed under "property sets" main menu item within this specification and from the object documentation sheet for those object to which they are applicable. The naming convention "Pset_Xxx" applies to all those property sets that are defined as part of the IFC specification and it shall be used as the value of the _Name_ attribute.

In addition any user defined property set can be captured. Property sets that are not declared as part of the IFC specification shall have a _Name_ value not including the "Pset_" prefix.