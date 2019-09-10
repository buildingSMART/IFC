An _IfcControllerType_ defines a particular type of controller that interacts with other devices in a control system such as a building automation control system.

> <font color="#0000ff" size="-1">
HISTORY: New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcControllerType_ provides for all forms of controller.

Usage of _IfcControllerType_ defines the parameters for one or more occurrences of _IfcDistributionControlElement_. Parameters are specified through property sets that may be enumerated in the _IfcControllerTypeEnum_ data type.

An _IfcController_ typically has a relationship with an _IfcSensor_ and/or an _IfcActuator_. These relationships can be handled either through aggregation (e.g., a unitized controller/actuator assembly) using _IfcRelAggregates_ or simply as an arbitrary grouping of related devices using the _IfcRelAssignsToGroup_ relationship.

****Property Set Use Definition****:

The property sets relating to the _IfcControllerType_ defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcControllerType_ are part of this IFC release:

* [Pset_ControllerTypeCommon](../../psd/IfcBuildingControlsDomain/Pset_ControllerTypeCommon.xml): property set for the properties common to all types of controller, if available 
* [Pset_ControllerTypeProportional](../../psd/IfcBuildingControlsDomain/Pset_ControllerTypeProportional.xml): specific property set for the properties of a proportional controller, if available 
* [Pset_ControllerTypeTwoPosition](../../psd/IfcBuildingControlsDomain/Pset_ControllerTypeTwoPosition.xml): specific property set for the properties of a two position controller, if available

In addition to the above, the following predefined property sets may be used for specification of input/output signal type for controllers:

* [Pset_AnalogInput](../../psd/IfcBuildingControlsDomain/Pset_AnalogInput.xml): specific property set for the properties of an analog input, if available 
* [Pset_AnalogOutput](../../psd/IfcBuildingControlsDomain/Pset_AnalogOutput.xml): specific property set for the properties of an analog output, if available
* [Pset_BinaryInput](../../psd/IfcBuildingControlsDomain/Pset_BinaryInput.xml): specific property set for the properties of a binary input, if available 
* [Pset_BinaryOutput](../../psd/IfcBuildingControlsDomain/Pset_BinaryOutput.xml): specific property set for the properties of a binary output, if available
* [Pset_MultiStateInput](../../psd/IfcBuildingControlsDomain/Pset_MultiStateInput.xml): specific property set for the properties of a multi-state input, if available 
* [Pset_MultiStateOutput](../../psd/IfcBuildingControlsDomain/Pset_MultiStateOutput.xml): specific property set for the properties of a multi-state output, if available

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.
