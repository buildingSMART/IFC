Architectural program for a space in the building or facility being designed; essentially the requirements definition for such a building space.

> <font size="-1">NOTE: that this 'program' defines the client
		requirements for the space before the building is designed. Space programs can
		change over the life cycle of a building, after the building is occupied.
		Changes to space programs take place in the facilities management/operations
		phase of the building life cycle.</font>

The assignment of a person or an organization to a space program, e.g., as the anticipated occupants of the space, is handled through using the objectified relationship _IfcRelAssignsToActor_ referring to _IfcActor_. Space programs can be nested, i.e. an IfcSpaceProgram can specify a program group up to any desired level. This is handled through using the objectified relationship _IfcRelNests_.

****Property Set Use Definition****:

The property sets relating to the _IfcSpaceProgram_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcSpaceProgram_ are part of this IFC release:

* [Pset_SpaceProgramCommon](../../psd/IfcArchitectureDomain/Pset_SpaceProgramCommon.xml){ target="SOURCE"}: common property set for all types of the space program

****General Use Definition****

The _IfcSpaceProgram_ entity is used to define:

* the architectural program for a space in the building or facility being designed; 
* the standard for space allocation that can be assigned to persons within an organization. 

As the architectural program, the _IfcSpaceProgram_ class sets down the requirements definition for a space in the building or facility being designed. Used in this way, it defines the client requirements for the space before the building in designed. Space programs can change over the life cycle of a building, after the building is occupied. Changes to space programs take place in the facilities management/operations phase of the building life cycle.

As a space standard for facilities management (FM), the _IfcSpaceProgram_ class defines the requirements for usage of a space according to the roles of persons that will occupy the space. This could take into account role driven elements such as whether the space should be a single person office, corner space, glazing on two sides etc. In order to use the class as an space standard within FM, a classification of spaces must have been established. This does not mean that each individual space needs to have a classification although for locating persons having an assigned space standard, this would be desirable.

> <font color="#0000CC" size="-1">HISTORY New Entity in IFC
		Release 1.0</font>