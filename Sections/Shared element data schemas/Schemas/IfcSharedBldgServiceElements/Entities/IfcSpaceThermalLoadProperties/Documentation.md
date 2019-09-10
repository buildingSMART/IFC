The space thermal load _IfcSpaceThermalLoadProperties_ defines all thermal losses and gains occurring within a space or zone. Those losses or gains can either be requirements (desired values) or criteria (actual values). The thermal load source attribute defines an enumeration of possible sources of the thermal load. The maximum, minimum, time series and applicable value ratio values are all interpreted according to the source. The maximum and minimum values should not be used if time series values are provided.

The _IfcSpaceThermalLoadProperties_ is a statically defined property set and should be attached to the instance(s) of _IfcSpace_ through the _IfcRelDefinesByProperties_ relationship. If there are several different thermal loads occurring within a space, multiple instances of _IfcSpaceThermalLoadProperties_ should be assigned.

> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC R2.0, has been renamed from IfcSpaceUseCase in IFC Release 2x.<br>
    	</font>
