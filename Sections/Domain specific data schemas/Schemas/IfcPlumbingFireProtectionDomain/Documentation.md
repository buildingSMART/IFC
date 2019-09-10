The _IfcPlumbingFireProtectionDomain_ schema forms part of the Domain Layer of the IFC Model. It extends the ideas concerning building services outlined in the _IfcSharedBldgServicesElements_ schema. It defines concepts in the domain of plumbing and fire protection.

### Scope
The scope of the _IfcPlumbingFireProtectionDomain_, in conjunction with other building services related schemata, is the provision of plumbing and fire protection services to buildings.

In the case of plumbing, the scope includes for the provision of services external to the building up to the final manhole at which connection is made to the public drainage/sewage service provision. Particular exceptions to support building code checking requirements are made as outlined in '**Additional Provisions**' as outlined below.

In the case of fire protection, the scope includes for all services from the point at which a fire authority service is connected or the point at which the statutory water provider terminates the public connection.

In particular, _IfcPlumbingFireProtectionDomain_ schema supports ideas including types of:

* sanitary element concerned with personal and public hygiene,
* trap on waste pipelines to prevent backflow and odour transmission,
* interceptor to capture unwanted liquid and solid waste materials and prevent their passage into drainage pipelines,
* waste disposal unit,
* cowl terminating ventilation and rainwater pipes at their highest elevation,
* automatic and manual terminal point that can be activated to extinguish fire,
* hydrant that provide a source of water for hoses in the event of fire or other need for a temporary water supply.

### Occurrence
Classes within this schema define types of elements that are used in plumbing and fire protection. They are defined either as subtypes of IfcTypeProduct or of other classes that are themselves subtypes of IfcTypeProduct.

The objective is that a particular type of element is defined once in an IFC exchange. Occurrences of elements conforming to a particular type are defined by using related subtypes of IfcDistributionElement. The following table shows the entities used for capturing the occurrence of a particular element type within this schema:

<table border="0">
  <tbody>
    <tr>
      <td>IfcFireSuppressionTerminalType</td>
      <td>IfcFlowTerminal</td>
    </tr>
    <tr>
      <td>IfcSanitaryTerminalType</td>
      <td>IfcFlowTerminal</td>
    </tr>
    <tr>
      <td>IfcStackTerminalType</td>
      <td>IfcFlowTerminal</td>
    </tr>
    <tr>
      <td>IfcWasteTerminalType</td>
      <td>IfcFlowTerminal</td>
    </tr>
  </tbody>
</table>

### Additional Provisions
Additional provisions are made to support main drainage/sewage requirements in the domain of building code checking by provision of the following property sets that may be used in conjunction with the entities identified:

<table border="0">
  <tbody>
    <tr>
      <td>Catchment</td>
      <td><a href="../../psd/IfcPlumbingFireProtectionDomain/Pset_DrainageCatchment.xml">Pset_DrainageCatchment</a></td>
      <td>IfcSpatialStructureElement</td>
    </tr>
    <tr>
      <td>Culvert</td>
      <td><a href="../../psd/IfcPlumbingFireProtectionDomain/Pset_DrainageCulvert.xml">Pset_DrainageCulvert</a></td>
      <td>IfcSystem</td>
    </tr>
    <tr>
      <td>Drainage reserve</td>
      <td><a href="../../psd/IfcPlumbingFireProtectionDomain/Pset_DrainageReserve.xml">Pset_DrainageReserve</a></td>
      <td>IfcSpatialStructureElement</td>
    </tr>
    <tr>
      <td>Outfall</td>
      <td><a href="../../psd/IfcPlumbingFireProtectionDomain/Pset_DrainageOutfall.xml">Pset_DrainageOutfall</a></td>
      <td>IfcProxy</td>
    </tr>
  </tbody>
</table>

These provisions are outside the declared scope of the schema and are not supported by explicit classes within the IFC 2x2 model. It is anticipated that further developments covering the provision of external works/public drainage and sewage provision will further provide for these capabilities in a future release of the IFC model.

> <font color="#0000ff" size="-1">HISTORY:
New schema in IFC 2x2</font>
>