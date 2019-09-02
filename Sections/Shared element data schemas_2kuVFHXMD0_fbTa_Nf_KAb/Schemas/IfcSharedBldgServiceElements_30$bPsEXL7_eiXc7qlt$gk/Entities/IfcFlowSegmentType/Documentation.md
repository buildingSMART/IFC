The element type _IfcFlowSegmentType_ defines a list of commonly shared property set definitions of a flow segment and an optional set of product representations. It is used to define a flow segment specification (the specific product information, that is common to all occurrences of that product type).

A flow segment type is used to define the common properties of a flow segment that may be applied to many occurrences of that type. A flow segment is a section of a distribution system, such as a duct, pipe, or conduit, that typically has only two ports. Flow segment types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

Occurrences of the _IfcFlowSegmentType_ are represented by instances of _IfcFlowSegment_ or its subtypes.

> HISTORY&nbsp; New entity in IFC2x2.

****Material Use Definition****

The material of the **IfcDistributionFlowSegmentType** is defined using one of the following entities:

* [IfcMaterialProfileSet](../../ifcmaterialresource/lexical/ifcmaterialprofileset.htm) : This defines the material cross section which may be used to generate the 'Body' representation at occurrences (for parametric definitions not having representation), or for analysis purposes.
* [IfcMaterialConstituentSet](../../ifcmaterialresource/lexical/ifcmaterialconstituentset.htm) : For elements containing multiple materials where profiles are not applicable, this indicates materials at named aspects. 
*  [IfcMaterial](../../ifcmaterialresource/lexical/ifcmaterial.htm) : For elements comprised of a single material where profiles are not applicable, this indicates the material.