The global unit assignment of the project defines the global units for measures and values when the units are not otherwise defined more specifically using entity type _IfcMeasureWithUnit_ as attribute's datatype.

An example where a project's global basic length, area, volume and time units are defined as SI units:

> 
> ```
> 
#1=IFCPROJECT ('00ZhrqZYLBcgy$rVVaiu2A', $, 'Example project', $, $, $, $, $, #2);  
> #2=IFCUNITASSIGNMENT ((#3, #4, #5, #6));  
> #3=IFCSIUNIT (\*, .LENGTHUNIT., .MILLI., .METRE.);  
> #4=IFCSIUNIT (\*, .AREAUNIT., $, .SQUARE_METRE.);  
> #5=IFCSIUNIT (\*, .VOLUMEUNIT., $, .CUBIC_METRE.);  
> #6=IFCSIUNIT (\*, .TIMEUNIT., $, .SECOND.);  
> 
> ```


> NOTE&nbsp; In the examples the '\*' character as the first value in the _IfcSIUnit_-instances is due to the fact that in the _IfcSIUnit_ the inherited attribute .Dimensions is redefined as a derived attribute. In the IFC Object Model schema there is a function that returns the derived dimensional exponent values for SI units. In the exchange file the derived attribute values are not exchanged, and in the case of redefinition the value is replaced by '\*'.

An example of a defined measure type with global unit assignment follows where the attribute IfcDoor.OverallWidth is of datatype IfcPositiveLengthMeasure without possibility of using specific unit from _IfcMeasureWithUnit_. Then the global unit for length measure applies; in this case metres:

> 
> ```
> 
#1=IFCPROJECT ('00ZhrqZYLBcgy$rVVaiu2A', $, 'Example project', $, $, $, $, $, #2);  
> #2=IFCUNITASSIGNMENT ((#3, #4, #5, #6));  
> #3=IFCSIUNIT (\*, .LENGTHUNIT., .MILLI., .METRE.);  
> #4=IFCSIUNIT (\*, .AREAUNIT., $, .SQUARE_METRE.);  
> #5=IFCSIUNIT (\*, .VOLUMEUNIT., $, .CUBIC_METRE.);  
> #6=IFCSIUNIT (\*, .TIMEUNIT., $, .SECOND.);  
> #7=IFCDOOR('00ZhrqZYLBcgy$rVVaiu2B', $, 'Door-1', $, $, $, $, $, 2., 1., $, $);  
> 
> ```


An example where a project's global basic length, area and volume units are defined as imperial units (inches, square feet and cubic feet), which are further defined as conversion based units relative to SI units millimeter, square meter and cubic meter:

> 
> ```
> 
#1=IFCPROJECT ('00ZhrqZYLBcgy$rVVaiu2B', $, 'Example project', $, $, $, $, $, #2);  
> #2=IFCUNITASSIGNMENT ((#6, #7, #10, #13));  
> #3=IFCSIUNIT (\*, .LENGTHUNIT., .MILLI., .METRE.);  
> #4=IFCSIUNIT (\*, .AREAUNIT., $, .SQUARE_METRE.);  
> #5=IFCSIUNIT (\*, .VOLUMEUNIT., $, .CUBIC_METRE.);  
> #6=IFCSIUNIT (\*, .TIMEUNIT., $, .SECOND.);  
> #7=IFCCONVERSIONBASEDUNIT(#9, .LENGTHUNIT., 'INCH', #8);  
> #8=IFCMEASUREWITHUNIT(IFCLENGTHMEASURE(25.4), #3);  
> #9=IFCDIMENSIONALEXPONENTS(1, 0, 0, 0, 0, 0, 0);  
> #10=IFCCONVERSIONBASEDUNIT(#11, .AREAUNIT., 'SQUARE_FEET', #12);  
> #11=IFCDIMENSIONALEXPONENTS(2, 0, 0, 0, 0, 0, 0);  
> #12=IFCMEASUREWITHUNIT(IFCAREAMEASURE(0.09290304), #4);  
> #13=IFCCONVERSIONBASEDUNIT(#14, .VOLUMEUNIT., 'CUBIC_FEET', #15);  
> #14=IFCDIMENSIONALEXPONENTS(3, 0, 0, 0, 0, 0, 0);  
> #15=IFCMEASUREWITHUNIT(IFCVOLUMEMEASURE(0.0283168466), #5);  
> 
> ```


In a conversion based unit the scaling factor, like 0.0283168466 for cubic feet, expresses how many base units make up one conversion based unit.

Another example of a conversion based unit would be the definition of temperature in degrees Fahrenheit. A conversion based unit should be used for this purpose, because degrees Fahrenheit can be defined using degrees Celsius. However, with _IfcConversionBasedUnit_ one cannot define their relationship fully because the zero degrees offset between them cannot be defined. Rather, the subtype _IfcConversionBasedUnitWithOffset_ is used to indicate such offset between degrees Fahrenheit and Celsius.

Yet another example of a conversion based unit would be degrees and gradians as a unit for plane angle measure. These can be defined as a conversion based unit based on radian unit.

An example definition of a unit for specific heat capacity (Joule / kg Kelvin), which is defined as a derived unit based on basic SI units.

> 
> ```
> 
#1=IFCPROJECT('00ZhrqZYLBcgy$rVVaiu2A', $, 'Example project', $, $, $, $, $, #2);  
> #2=IFCUNITASSIGNMENT((#3, #4, #5, #6, #7, #8, #9, #10));  
> #3=IFCSIUNIT(\*, .LENGTHUNIT., .MILLI., .METRE.);  
> #4=IFCSIUNIT(\*, .AREAUNIT., $, .SQUARE_METRE.);  
> #5=IFCSIUNIT(\*, .VOLUMEUNIT., $, .CUBIC_METRE.);  
> #6=IFCSIUNIT(\*, .TIMEUNIT., $, .SECOND.);  
> #7=IFCSIUNIT(\*, .ENERGYUNIT., $, .JOULE.);  
> #8=IFCSIUNIT(\*, .MASSUNIT., .KILO., .GRAM.);  
> #9=IFCSIUNIT(\*, .THERMODYNAMICTEMPERATUREUNIT., $, .KELVIN.);  
> #10=IFCDERIVEDUNIT((#11, #12, #13), .SPECIFICHEATCAPACITYUNIT., $);  
> #11=IFCDERIVEDUNITELEMENT(#7, 1);  
> #12=IFCDERIVEDUNITELEMENT(#8, -1);  
> #13=IFCDERIVEDUNITELEMENT(#9, -1);  
> 
> ```
