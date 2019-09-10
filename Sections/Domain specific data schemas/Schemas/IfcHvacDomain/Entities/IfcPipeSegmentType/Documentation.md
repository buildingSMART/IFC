The element type _IfcPipeSegmentType_ defines a list of commonly shared property set definitions of a pipe segment and an optional set of product representations. It is used to define a pipe segment specification (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">
		NOTE: The product representations are defined as
		representation maps (at the level of the supertype <i>IfcTypeProduct</i>, which
		get assigned by an element occurrence instance through the
		<i>IfcShapeRepresentation.Item[1]</i> being an
		<i>IfcMappedItem</i>.
    	</font>

A pipe segment type is used to define the common properties of a pipe segment that may be applied to many occurrences of that type. A pipe segment is used to typically join two sections of a piping network. Pipe segment types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcPipeSegmentType_ are represented by instances of _IfcFlowSegment_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_PipeSegmentTypeCommon](../../psd/IfcHvacDomain/Pset_PipeSegmentTypeCommon.xml){ target="SOURCE"}: common property set for all pipe segment types 
    * [Pset_PipeSegmentTypeGutter](../../psd/IfcHvacDomain/Pset_PipeSegmentTypeGutter.xml){ target="SOURCE"}: property set for all gutter segment types 


> <font color="#0000ff" size="-1">
    	HISTORY: New entity in IFC Release 2x2.<br>
    	</font>