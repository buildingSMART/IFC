An _IfcZone_ is a spatial system under which individual _IfcSpace_'s (and other _IfcZone_'s) are grouped. In contrary to the _IfcSpatialZone_ entity, _IfcZone_ is a mere grouping, it can not define an own geometric representation and placement. Therefore it cannot be used for spatial zones having a different shape and size compared to the shape and size of aggregated spaces.

> NOTE&nbsp; The _IfcZone_ is regarded as the spatial system (as compared to the building service, electrical, or analytical system), the name remains _IfcZone_ for compatibility reasons, instead of using a proper naming convention, like IfcSpatialSystem.

> NOTE&nbsp; One of the purposes of a zone is to define a fire compartmentation. In this case it defines the geometric information about the fire compartment (through the contained spaces) and information, whether this compartment is ventilated or sprinkler protected. In addition the fire risk code and the hazard type can be added, the coding is normally defined within a national fire regulation. All that information is available within the relevant property sets. Again, if an independent shape has to be provided to the fire compartment, then the entity _IfcSpatialZone_ shall be used.

In case of a zone denoting a (fire) compartment, the following types should be used, if applicable, as values of the _ObjectType_ attribute:

* **'FireCompartment'**: a zone of spaces, collected to represent a single fire compartment.
* **'ElevatorShaft'**: a collection of spaces within an elevator, potentially going through many storeys.
* **'RisingDuct'**: A collection of vertical airspaces.
* **'RunningDuct'**: A collection of horizontal airspaces.