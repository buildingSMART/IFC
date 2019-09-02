Slab types may be described at several levels of detail to support the following slab occurrences:

* _IfcSlab_: Explicit geometry instantiated in exact form at occurrences.
* _IfcSlabStandardCase_: Implicit material layers filling boundary ('FootPrint' representation) defined at occurrences.
* _IfcSlabElementedCase_: implicit material layers and corresponding aggregated parts filling each layer.

As shown in Figure 1, each material layer may be elaborated into an element (where the Name matches exactly), and each element may be defined by its own type, which may be further elaborated by material layers and/or parts. The _LayerThickness_ of _IfcMaterialLayer_ must be derived from the corresponding element as follows:

* if element does not have a type, then the thickness must be regarded as 0 (supporting scenario where a particular configuration may have one side a wall unfinished) 
* if element has a material layer set, then it must equal the total thickness of the element's material layer set
* if element has a material profile set, then it must equal the total thickness of the element's material profile set
* if element is decomposed into parts (such as _IfcElementAssemblyType_ for slab framing), then it must equal the bounding extent of the parts according to the layer set direction - if parts do not have representations, then such thickness is calculated according to the material layers or profiles.

!["voiding"](../../../figures/ifcslabtype-floor.png "Figure 1 &mdash; Slab type")