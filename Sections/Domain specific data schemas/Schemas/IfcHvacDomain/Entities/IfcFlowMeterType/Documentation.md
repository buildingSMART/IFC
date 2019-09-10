The element type _IfcFlowMeterType_ defines a list of commonly shared property set definitions of a flow meter and an optional set of product representations. It is used to define a flow meter specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A flow meter type is used to define the common properties of a flow meter that may be applied to many occurrences of that type. A flow meter is a device that is used to measure the flow rate in a system. flow meter types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcFlowMeterType_ are represented by instances of _IfcFlowController_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_FlowMeterTypeCommon](../../psd/IfcHvacDomain/Pset_FlowMeterTypeCommon.xml){ target="SOURCE"}: common property set for all flow meter types 
    * [Pset_FlowMeterTypeEnergyMeter](../../psd/IfcHvacDomain/Pset_FlowMeterTypeEnergyMeter.xml){ target="SOURCE"}: property set for all flow meter types that are used to measure the flow of energy 

    * [Pset_FlowMeterTypeGasMeter](../../psd/IfcHvacDomain/Pset_FlowMeterTypeGasMeter.xml){ target="SOURCE"}: property set for all flow meter types that are used to measure the flow of gas 

    * [Pset_FlowMeterTypeOilMeter](../../psd/IfcHvacDomain/Pset_FlowMeterTypeOilMeter.xml){ target="SOURCE"}: property set for all flow meter types that are used to measure the flow of oil 

    * [Pset_FlowMeterTypeWaterMeter](../../psd/IfcHvacDomain/Pset_FlowMeterTypeWaterMeter.xml){ target="SOURCE"}: property set for all flow meter types that are used to measure the flow of water 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
