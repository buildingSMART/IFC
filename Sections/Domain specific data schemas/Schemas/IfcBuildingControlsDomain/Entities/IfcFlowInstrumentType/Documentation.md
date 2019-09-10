An _IfcFlowInstrumentType_ defines a particular type of flow instrument that reads and displays the value of a particular property of a system at a point, or that displays the difference in the value of a property between two points.

> <font color="#0000ff" size="-1">HISTORY:
New entity in IFC 2x2</font>
> 


****Use Definitions****

An _IfcFlowInstrumentType_ provides for all forms of mechanical flow instrument (thermometers, pressure gauges etc.) and electrical flow instruments (ammeters, voltmeters etc.)

Usage of _IfcFlowInstrumentType_ defines the parameters for one or more occurrences of _IfcDistributionControlElement_. Parameters for mechanical flow instruments are specified through property sets that are enumerated in the _IfcFlowInstrumentTypeEnum_ data type. Property sets for electrical flow instruments are not yet defined.

****Property Set Use Definition****:

The property sets relating to the _IfcFlowInstrumentType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcFlowInstrumentType_ are part of this IFC release:

* [Pset_FlowInstrumentTypeThermometer](../../psd/IfcBuildingControlsDomain/Pset_FlowInstrumentTypeThermometer.xml): specific property set for the properties of a thermometer, if available 
* [Pset_FlowInstrumentTypePressureGauge](../../psd/IfcBuildingControlsDomain/Pset_FlowInstrumentTypePressureGauge.xml): specific property set for the properties of a pressure gauge, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.