The _IfcBuildingControlsDomain_ schema forms part of the Domain Layer of the IFC Model. It extends the ideas concerning building services outlined in the _IfcSharedBldgServicesElements_ schema. It defines concepts of building automation, control, instrumentation and alarm.

### Scope
The _IfcBuildingControlsDomain_ schema supports ideas including types of:

* actuator,
* alarm,
* controller,
* sensor,
* flow instrument ,

Elements that perform the control action such as valves and dampers are principally types of distribution element and are located principally in the _IfcSharedBldgServicesElements_ schema

### Occurrence
Classes within this schema define types of elements that are used in building automation, control and instrumentation. They are defined either as subtypes of _IfcTypeProduct_ or of other classes that are themselves subtypes of _IfcTypeProduct_.

The objective is that a particular type of element is defined once in an IFC exchange. Instances or occurrences of elements conforming to a particular type are defined by instances of related subtypes of _IfcDistributionElement_. The following table sets down the class used for capturing the occurrence of a particular element type within this schema:

<table border="0">
  <tbody>
    <tr>
      <td width="150">IfcActuatorType</td>
      <td>IfcDistributionControlElement</td>
    </tr>
    <tr>
      <td width="150">IfcAlarmType</td>
      <td>IfcDistributionControlElement</td>
    </tr>
    <tr>
      <td width="150">IfcControllerType</td>
      <td>IfcDistributionControlElement</td>
    </tr>
    <tr>
      <td width="150">IfcFlowInstrumentType</td>
      <td>IfcDistributionControlElement</td>
    </tr>
    <tr>
      <td width="150">IfcSensorType</td>
      <td>IfcDistributionControlElement</td>
    </tr>
  </tbody>
</table>

> <font color="#0000ff" size="-1">HISTORY:
New schema in IFC 2x2</font>
>