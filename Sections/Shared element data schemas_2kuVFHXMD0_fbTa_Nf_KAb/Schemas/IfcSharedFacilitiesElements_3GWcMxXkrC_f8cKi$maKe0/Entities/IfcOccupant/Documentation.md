An_IfcOccupant_ is a type of actor that defines the form of occupancy of a property.

> <font color="#0000ff" size="-1">HISTORY
New class in IFC Release 2x. Modified in IFC 2x2</font>

### Use Definitions
The principal purpose of _IfcOccupant_ is to determine the nature of occupancy of a property for a particular actor. All characteristics relating to the actor (name, organization details etc.) are inherited from the _IfcActor_ class.

The property to be occupied is defined by _IfcSpatialStructureElement_ and the assignment of the occupant to the property is via the _IfcRelOccupiesSpaces_ relationship class. Particular details of the agreement relating to the occupancy of a property are dealt with in the [Pset_PropertyAgreement](../../psd/IfcSharedFacilitiesElements/Pset_PropertyAgreement.xml) that is defined for the instance of _IfcSpatialStructureElement_. This means that an occupant may be related to a site, building, building storey or space or to any composition of site, building, building storey or space through the _IfcSpatialStructureElement.ElementComposition_. For instance, if the property concerned is several office spaces on a building storey, it might be appropriate to reference _IfcBuildingStorey.ElementComposition=PARTIAL_.

Occupants of a property may be considered to be the parties to an agreement. The roles that the occupant may play in respect to an agreement are defined in the _IfcOccupantTypeEnum_. If the role is not specified by the predefined contents of this enumeration, the value USERDEFINED may be set and the _IfcOccupant.UserDefinedOccupant_ attribute asserted.

![Image](figures/IfcOccupant-Fig1.gif)