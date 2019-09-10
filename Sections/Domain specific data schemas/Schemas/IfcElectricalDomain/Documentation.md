The _IfcElectricalDomain_ schema forms part of the Domain Layer of the IFC Model. It extends the ideas concerning building services outlined in the _IfcSharedBldgServicesElements_ schema. It defines concepts of electrical supply and provision and concepts of light fixtures and illuminance within buildings.

### Scope
The scope of the IfcElectrical domain is defined as:

1. low voltage electrical installations from 12V (AC/DC) to 1000V (AC) or 1500 volts (DC) in accordance with IEC definitions where installations in scope are considered to commence at a meter where the public utility supply terminates or at a transformer where voltage is stepped down to the low voltage range in scope,
2. connection of equipment to circuits, distribution points etc,
3. steady state operation of electrical installations,
4. light fixtures (fittings), their types and the provision of such information as is necessary to enable lighting calculations that provide physically accurate illuminance.

The _IfcElectricalDomain_ schema supports ideas including types of:

* cable carrier fittings (for conduit, cable tray, cable duct and ladder),
* electrical appliance,
* electric heater,
* electric motor,
* distribution points including various types of control, mimic and indicator panels,
* generator,
* junction box,
* light fixture,
* lamp,
* outlet,
* protective device,
* switching device,
* transformer,

#### Out of Scope
The following are deemed to be out of scope of the _IfcElectricalDomain_ schema at this time:

* medium and high voltage installations over 1000 volts AC and 1500 volts DC
* systems with voltage of less than 12 volts (AC/DC)
* public utility supply of electrical services
* path of cables/conductors (other than as logical paths identifying connection sequence)
* cable routers (cable ladders)
* electrical appliances like fax machines, phones, printers etc other than as defined as electric appliances for the purposes of identification.
* non steady state/transient states of operation of electrical installations
* security arrangements associated with safety of electrical installations
* communication signals between automation devices or bus systems
* sensors (which are dealt with in the IfcBuildingControl domain schema)
* computer network cabling and devices used on networks
* spotlight mirror systems whereby a spotlight is directed towards a distant mirror that the distributes the light energy (other than as a group of separately defined objects)
* lighting for specialist purposes (e.g. stage, painting, etc.) 
* properties and provisions that enable the visual display or rendering of surfaces under illuminance (rendering, as in VRML, and photo accurate simulation are within the scope of the _IfcPresentationResource_ schema.

### Occurrence
Many classes within this schema define types of elements that are used in electrical building services. They are defined either as subtypes of IfcTypeProduct or of other classes that are themselves subtypes of IfcTypeProduct.

The objective is that a particular type of element is defined once in an IFC exchange. Occurrences of elements conforming to a particular type are defined by instances of related subtypes of IfcDistributionElement. Details of the relevant occurrence subtype are provided in the documentation for the type class.

### Electrical Circuit
Electrical devices form part of an electrical circuit. An instance of an electrical circuit is defined as a named instance of IfcSystem.

> <font color="#0000FF" size="-1"> HISTORY:New schema in
		  IFC Release 2x.  </font>
>
