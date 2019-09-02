This enumeration identifies different types of distribution systems. It is used to designate systems by their function as well as ports of devices within such systems to restrict connectivity to compatible connections.

> HISTORY&nbsp; New enumeration in IFC4.

{ .spec-head}
Enumerated Item Definitions:

#### Pipe-based systems and ports
Ports for pipes may be connected using _IfcPipeSegment_ and _IfcPipeFitting_. Type objects for pipe segments and fittings (_IfcPipeSegmentType_ and _IfcPipeFittingType_) that are not specific to a particular system type may have ports with _PredefinedType_ of NOTDEFINED which indicates that occurrences of such objects may connect to any other pipe-based port (but not cable-based or duct-based). Upon connection to a device within a system, then such port should have its PredefinedType set to that of the connecting port.

> EXAMPLE&nbsp; An _IfcPipeSegmentType_ may be designated as NOTDEFINED, as it may support hot water, cold water, or any other fluid. When an instance of a pipe is instantiated in a building, then it may be connected to any other pipe-based port (using either a pipe-based enumeration or NOTDEFINED). Upon connection within a building, then such port should be marked according to its use such as DOMESTICCOLDWATER.

Valid enumerations for pipes and related elements include:

* **CHEMICAL**: Arbitrary chemical further qualified by property set, such as for medical or industrial use.
* **CHILLEDWATER**: Nonpotable chilled water, such as circulated through an evaporator.
* **COMPRESSEDAIR**: Compressed air system.
* **CONDENSERWATER**: Nonpotable water, such as circulated through a condenser.
* **CONVEYING**: Arbitrary supply of substances.
* **DISPOSAL**: Arbitrary disposal of substances.
* **DOMESTICCOLDWATER**: Unheated potable water distribution system.
* **DOMESTICHOTWATER**: Heated potable water distribution system.
* **DRAINAGE**: Drainage collection system.
* **FIREPROTECTION**: Fire protection sprinkler system.
* **FUEL**: Arbitrary supply of fuel.
* **GAS**: Gas-phase materials such as methane or natural gas.
* **HAZARDOUS**: Hazardous material or fluid collection system.
* **HEATING**: Water or steam heated from a boiler and circulated through radiators.
* **MUNICIPALSOLIDWASTE**: Items consumed and discarded, commonly known as trash or garbage.
* **OIL**: Oil distribution system.
* **OPERATIONAL**: Operating supplies system.
* **RAINWATER**: Rainwater resulting from precipitation which directly falls on a parcel.
* **REFRIGERATION**: Refrigerant distribution system for purposes of fulfilling all or parts of a refrigeration cycle.
* **SEWAGE**: Sewage collection system.
* **STORMWATER**: Stormwater resulting from precipitation which runs off or travels over the ground surface.
* **VACUUM**: Vacuum distribution system.
* **VENT**: Vent system for wastewater piping systems.
* **WASTEWATER**: Water adversely affected in quality by anthropogenic influence, possibly originating from sewage, drainage, or other source.
* **WATERSUPPLY**: Arbitrary water supply.

> NOTE&nbsp; Drainage systems that receive sources from multiple types should be designated according to priority in the following order: RAINWATER, STORMWATER, DRAINAGE, SEWAGE, WASTEWATER, HAZARDOUS. For example, a WASTEWATER system may have SEWAGE as a source but not HAZARDOUS (in the absense of treatment equipment in between).

#### Duct-based systems and ports
Ports for ducts may be connected using _IfcDuctSegment_ and _IfcDuctFitting_. Type objects for duct segments and fittings (_IfcDuctSegmentType_ and _IfcDuctFittingType_ that are not specific to a particular system type may have ports with _PredefinedType_ of NOTDEFINED which indicates that occurrences of such objects may connect to any other duct-based port (but not pipe-based or cable-based). Upon connection to a device within a system, then such port should have its PredefinedType set to that of the connecting port.

> EXAMPLE&nbsp; An _IfcDuctSegmentType_ may be designated as NOTDEFINED, as it may support air conditioning, recirculation, or exhaust. When an instance of a duct is instantiated in a building, then it may be connected to any other duct-based port (using either a duct-based enumeration or NOTDEFINED). Upon connection within a building, then such port should be marked according to its use such as AIRCONDITIONING.

Valid enumerations for ducts and related elements include:

* **AIRCONDITIONING**: Conditioned air distribution system for purposes of maintaining a temperature range within one or more spaces.
* **EXHAUST**: Exhaust air collection system for removing stale or noxious air from one or more spaces.
* **VENTILATION**: Ventilation air distribution system involved in either the exchange of air to the outside as well as circulation of air within a building.

> NOTE&nbsp; Ducts, equipment, and diffusers on the supply side (whether for heating, cooling, and/or air circulation) are considered AIRCONDITIONING; return air terminals, outside air intakes, ducts, and equipment for air that may be recirculated or exhausted are considered VENTILATION; return air terminals, ducts, and equipment for air that must be exhausted are considered EXHAUST.

#### Cable-based systems and ports
Ports for cables may be connected using _IfcCableSegment_ and _IfcCableFitting_. Type objects for cable segments and fittings (_IfcCableSegmentType_ and _IfcCableFittingType_ that are not specific to a particular system type may have ports with _PredefinedType_ of NOTDEFINED which indicates that occurrences of such objects may connect to any other cable-based port (but not pipe-based or duct-based). Upon connection to a device within a system, then such port should have its PredefinedType set to that of the connecting port.

> EXAMPLE&nbsp; An _IfcCableSegmentType_ for CAT-5 wiring may be designated as NOTDEFINED, as it may support transporting telephone, audio-visual, generic data, or even power. When an instance of a cable is instantiated in a building, then it may be connected to any other cable-based port (using either a cable-based enumeration or NOTDEFINED). Upon connection within a building, then such port should be marked according to its use such as DATA.

Valid enumerations for cables and related elements include:

* **AUDIOVISUAL**: A transport of a single media source, having audio and/or video streams.
* **CONTROL**: A transport or network dedicated to control system usage.
* **DATA**: A network having general-purpose usage.
* **EARTHING**: A path for equipotential bonding, conducting current to the ground.
* **ELECTRICAL**: A circuit for delivering electrical power.
* **ELECTROACCOUSTIC**: An amplified audio signal such as for loudspeakers.
* **LIGHTING**: A circuit dedicated for lighting, such as a fixture having sockets for lamps.
* **LIGHTNINGPROTECTION**: A path for conducting lightning current to the ground.
* **POWERGENERATION**: A path for power generation.
* **SECURITY**: A transport or network dedicated to security system usage.
* **SIGNAL**: A raw analog signal, such as modulated data or measurements from sensors.
* **TELEPHONE**: A transport or network dedicated to telephone system usage.
* **TV**: A transport of multiple media sources such as analog cable TV, satellite TV, or over-the-air TV.

> NOTE&nbsp; Cable ports used for communication do not necessarily require physical connection; they may also take the form of wireless radio transmission.

#### Cable Carriers
Ports for cable carriers may be connected using _IfcCableCarrierSegment_ and _IfcCableCarrierFitting_. Type objects for cable carrier segments and fittings (_IfcCableCarrierSegmentType_ and _IfcCableCarrierFittingType_ that are not specific to a particular system type may have ports with _PredefinedType_ of NOTDEFINED which indicates that occurrences of such objects may connect to ports of any other cable-carrier based port. Valid enumerations for cable carriers are the same as that for cables, and may be asserted if ports of the contained cables are all of the same type.