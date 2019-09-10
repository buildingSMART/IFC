The element type _IfcValveType_ defines a list of commonly shared property set definitions of a valve and an optional set of product representations. It is used to define a valve specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>) which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A valve type is used to define the common properties of a valve that may be applied to many occurrences of that type. Valves are typically is used in a building services piping distribution system to control or modulate the flow of the fluid. Valve types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcValveType_ are represented by instances of _IfcFlowController_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_ValveTypeCommon](../../psd/IfcHvacDomain/Pset_ValveTypeCommon.xml){ target="SOURCE"}: common property set for all valve types 
    * [Pset_ValveTypeAirRelease](../../psd/IfcHvacDomain/Pset_ValveTypeAirRelease.xml){ target="SOURCE"}: property set for air release valve types 

    * [Pset_ValveTypeDrawOffCock](../../psd/IfcHvacDomain/Pset_ValveTypeDrawOffCock.xml){ target="SOURCE"}: property set for draw off cock valve types 

    * [Pset_ValveTypeFaucet](../../psd/IfcHvacDomain/Pset_ValveTypeFaucet.xml){ target="SOURCE"}: property set for faucet valve types 

    * [Pset_ValveTypeFlushing](../../psd/IfcHvacDomain/Pset_ValveTypeFlushing.xml){ target="SOURCE"}: property set for flushing valve types 

    * [Pset_ValveTypeGasTap](../../psd/IfcHvacDomain/Pset_ValveTypeGasTap.xml){ target="SOURCE"}: property set for gas tap valve types 

    * [Pset_ValveTypeIsolating](../../psd/IfcHvacDomain/Pset_ValveTypeIsolating.xml){ target="SOURCE"}: property set for isolating valve types 

    * [Pset_ValveTypeMixing](../../psd/IfcHvacDomain/Pset_ValveTypeMixing.xml){ target="SOURCE"}: property set for mixing valve types 

    * [Pset_ValveTypePressureReducing](../../psd/IfcHvacDomain/Pset_ValveTypePressureReducing.xml){ target="SOURCE"}: property set for pressure reducing valve types 

    * [Pset_ValveTypePressureRelief](../../psd/IfcHvacDomain/Pset_ValveTypePressureRelief.xml){ target="SOURCE"}: property set for pressure relief valve types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>
