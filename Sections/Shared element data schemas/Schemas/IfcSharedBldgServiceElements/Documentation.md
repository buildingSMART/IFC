The _IfcSharedBldgServiceElements_ schema in the interoperability layer defines basic concepts required for interoperability primarily between Building Service domain extensions, notably _IfcHvacDomain_, _IfcPlumbingFireProtectionDomain_, _IfcElectricalDomain_ and _IfcBuildingControlsDomain_. This schema includes concepts such as basic type and occurrence definitions for flow and distribution systems and fundamental properties commonly used in building service scenarios (such as fluid-flow properties, electrical properties, space thermal properties, etc.)

The _IfcSharedBldgServiceElements_ schema heavily utilizes the concepts of type, occurrence and performance, as shown in Figure 1 below. Types are specializations of _IfcDistributionElementType_ while occurrences are specializations of _IfcDistributionElement_. Generally, only types are further elaborated in the domain schemas to provide the necessary specificity unique to each type. A third theme, defined in the _IfcControlExtension_ schema, relates to the performance characteristics of an occurrence utilizing instances of the _IfcPerformanceHistory_ entity.

!["type, occurrence and performance history concepts"](../../../../figures/ifcdistributionport_conceptslide2.gif "> <font color="#0000ff" size="-1">
Figure 1: A type can have zero or many occurrences. Each occurrence can have many performance history entities associated with it, allowing data that is specific to a certain phase of the lifecycle to be captured and maintained throughout the life of the dataset.
	    </font>")

The _IfcSharedBldgServiceElements_ schema specializes building services concepts symmetrically for occurrences and types, with the _primary_ functional role of the entity determining its classification into the following generic concepts:

* **Distribution Chamber**: a formed volume used in a distribution system, such as a sump, trench or manhole.
* **Energy Conversion Device**: a building systems device that converts energy from one form into another such as a boiler (i.e., combusting gas to heat water), chiller (i.e., using a refrigeration cycle to cool a liquid), or a cooling coil (i.e., using the phase-change characteristics of a refrigerant to cool air).
* **Flow Controller**: a device that regulates flow within a distribution system, such as a valve in a piping system, modulating damper in an air distribution system, or electrical switch in an electrical distribution system.
* **Flow Fitting**: a device that is used to interconnect flow segments or other fittings within a distribution system, such as a tee in a ducted system that branches flow into two directions, a junction box in an electrical distribution system, etc.
* **Flow Moving Device**: a device that is used to produce a pressure differential in a distribution system, such as a pump, fan, compressor, etc.
* **Flow Segment**: a section of a distribution system, such as a duct, pipe, conduit, etc.
* **Flow Storage Device**: a device used for the temporary storage of a fluid such as a liquid or a gas (e.g., tank), the voltage potential induced by the induced electron flow (e.g., a battery), etc.
* **Flow Terminal**: acts as a terminus or beginning element in a distribution system such as a ceiling register in a ducted air distribution system, a sink in a waste-water system, or a light fixture in an electrical lighting system.
* **Flow Treatment Device**: a device used to change the physical properties of the medium, such as an air, oil or water filter (used to remove particulates from the fluid), duct silencer (used to attenuate noise), etc.

Refer to the domain schemas where types are further elaborated utilizing the PredefinedType enumerations for examples of the range of supported concepts within these broad classifications. If a new type is needed within this classification, extend using the ElementType attribute. However, if a completely new concept is required that does not fit within this classification, utilize instances of the generic _IfcDistributionElementType_ and _IfcDistributionElement_ entities for the type/occurrence objects as needed.

Occurrences in a distribution system are typically coupled together using instances of _IfcDistributionPort_. This is also where concepts such as mass-flow properties (using instances of _IfcFluidFlowProperties_) are applied based on performance characteristics. Refer to the _IfcDistributionPort_ documentation within this schema for further elaboration on coupling together components in a distribution system and tracking the flow characteristics across the port boundaries.

> <font color="#0000ff" size="-1">
        HISTORY
        This schema has been significantly modified in 
        IFC Release 2x2. Refer to the change log and
        issues resolution database for details.
	    </font>