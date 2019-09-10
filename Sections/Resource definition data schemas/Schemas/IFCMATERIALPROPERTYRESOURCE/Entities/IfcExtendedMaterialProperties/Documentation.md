A container class for user defined properties of associated material. This provides a mechanism to assign properties that have not been defined in IFC specification.

> <font size="-1"><p> EXAMPLE: A set of extended material properties for energy calculation 

purposes can be defined as:</p>

<table align="Center" border="2" cellspacing="0" cellpadding="0" width="100%">
<th>Extended Material Properties for Energy Calculation</th>
</table><table border="1" width="100%">
  <tr>
    <td>
    <b>PropertyName</b>
    </td>
    <td>
    <b>Datatype</b>
    </td>
    <td>
    <b>Unit</b>
    </td>
    <td>
    <b>Description</b>
    </td>
  </tr>
  <tr>
    <td>
    ViscosityTemperatureDerivative
    </td>
    <td>
    REAL
    </td>
    <td>
    kg/m-s-K
    </td>
    <td>
    Viscosity temperature derivative.
    </td>
  </tr>
  <tr>
    <td>
    MoistureCapacityThermalGradient
    </td>
    <td>
    REAL
    </td>
    <td>
    kg/kg-K
    </td>
    <td>
    Thermal gradient coefficient for moisture capacity. Based on water vapor density.
    </td>
  </tr>
  <tr>
    <td>
    ThermalConductivityTemperatureDerivative
    </td>
    <td>
    REAL
    </td>
    <td>
    W/m-K2
    </td>
    <td>
    Thermal conductivity temperature derivative.
    </td>
  </tr>
  <tr>
    <td>
    SpecificHeatTemperatureDerivative
    </td>
    <td>
    REAL
    </td>
    <td>
    J/kg-K2
    </td>
    <td>
    Specific heat temperature derivative.
    </td>
  </tr>
  <tr>
    <td>
    VisibleRefractionIndex
    </td>
    <td>
    REAL
    </td>
    <td>
    -
    </td>
    <td>
    Index of refraction (visible) defines the "bending" of the solar ray in the visible spectrum when it 

passes from one medium into another.
    </td>
  </tr>
  <tr>
    <td>
    SolarRefractionIndex
    </td>
    <td>
    REAL
    </td>
    <td>
    -
    </td>
    <td>
    Index of refraction (solar) defines the "bending" of the solar ray when it passes from one medium 

into another.
    </td>
  </tr>
  <tr>
    <td>
    GasPressure
    </td>
    <td>
    REAL
    </td>
    <td>
    Pa
    </td>
    <td>
    Fill pressure (e.g. for between-pane gas fills): the pressure exerted by a mass of gas confined in a 

constant volume.
    </td>
  </tr>

</table>

</font>

> <font color="#0000FF" size="-1">HISTORY: New entity in Release IFC2x.</font>
