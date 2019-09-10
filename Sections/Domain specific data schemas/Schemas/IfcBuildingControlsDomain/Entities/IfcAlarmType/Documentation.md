The _IfcAlarmType_ defines a device that signals the existence of a condition or situation that is outside the boundaries of normal expectation or that activates such a device.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcAlarmType_ may be included into the spatial context of the building model through an (or multiple) instances of _IfcDistributionControlElement_.

Usage of _IfcAlarmType_ defines the parameters for one or more occurrences of _IfcDistributionControlElement_.

Alarm types include the provision of break glass buttons and manual pull boxes that are used to activate alarms. These should be used for alarms rather than a 'user defined' type of _IfcSwitchingDevice_.

****Property Set Use Definition****:

There are no predefined property sets for _IfcAlarmType_ in this release

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.
