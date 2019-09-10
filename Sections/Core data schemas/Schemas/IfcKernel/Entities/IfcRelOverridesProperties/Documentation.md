The objectified relationship (_IfcRelOverridesProperties_) defines the relationships between objects and a standard property set. It also defines a set of properties, which values override the standard values given within the standard property set.

The inherited attributes should be interpreted as follows:

* _SELF\IfcRelDefinedByProperties.RelatingPropertyDefinition_: Property set, which defines the standard set of properties assigned to all objects, that have the same set of properties,
* _SELF\IfcRelDefines.RelatedObjects_: An object occurrence, to which the same set of properties is applied. The object is characterized that certain property values, given by the standard set of properties, have a different value than those defined for all objects of the same style,
* _OverridingProperties_: A set of properties, that have a different value for the subset of objects. The set of the individual overriding properties have to correspond with a standard property set and its containing properties, as given by the _RelatingPropertyDefinition_ attribute. The correspondence is established by the _Name_ attribute.

It is provided as specialization of _IfcRelDefinedByProperties_ relationship.

> <font size="-1">NOTE that there must be a correspondence between the
		  names of the properties in the set of overriding properties and the names of
		  the properties whose values are to be changed in the base property set. In
		  addition the inherited attribute RelatingPropertyDefinition points to the
		  property set which values are overridden.</font>
>

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC Release
		  2x.</font>
>