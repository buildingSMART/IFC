The _IfcHvacDomain_ schema in the domain layer defines basic object concepts required for interoperability within the heating, ventilating and air conditioning (HVAC) domain. It extends concepts defined in the _IfcSharedBldgServiceElements_ schema.

### Scope
The scope of the _IfcHvacDomain_ schema is defined as:

1. The segments, fittings and connections that constitute duct and piping distribution systems typically used for building services, such as for air conditioning, ventilation and exhaust-air systems; chilled water, steam and heating hot water, potable water, waste, natural gas and LPG systems, etc.
2. Equipment typically used in building services systems, such as boilers, chillers, fans, pumps, etc., and the vibration isolation associated with these components.
3. Terminal and flow control devices, such as air vents and grilles, variable air volume modulators, valves, dampers, etc.

### Out of Scope
The following are deemed to be out of scope of the _IfcHvacDomain_ schema at this time:

* Industrial and institutional specialty equipment such as that used for power production, manufacturing and fabrication, etc.
* Provisions for dealing explicitly with hazardous materials such as chemical or biological agents
* Controls systems and sequencing systems for these equipment beyond what is defined in the _IfcBuildingControl_ domain schema

### Occurrence
Classes within this schema define only types of elements that are used in heating, ventilating and air conditioning building services where subtypes of _IfcDistributionElementType_ have been elaborated in the _IfcSharedBldgServiceElements_ schema to mirror their corresponding occurrence entities. Refer to the schema description for the _IfcSharedBldgServiceElements_ for more information about concepts of type, occurrence and performance history.

The objective is that a specific element type is defined only once in an IFC exchange. Occurrences of elements that are related to these types are defined by instances of related subtypes of _IfcDistributionElement_ (also defined in the _IfcSharedBldgServiceElements_ schema). Details of the relevant occurrence subtype are provided in the documentation for each type.

> <font color="#0000ff" size="-1">
    HISTORY
    This schema has been significantly modified in IFC R2x2. Refer to the change log and
    issues resolution database for details.
	</font>
