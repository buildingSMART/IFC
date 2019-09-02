A slab is a component of the construction that normally encloses a space vertically. The slab may provide the lower support (floor) or upper construction (roof slab) in any space in a building.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1  
> thick, flat or shaped component, usually larger than 300 mm square, used to form a covering or projecting from a building.

Only the core or constructional part of this construction is considered to be a slab. The upper finish (flooring, roofing) and the lower finish (ceiling, suspended ceiling) are considered to be coverings. A special type of slab is the landing, described as a floor section to which one or more stair flights or ramp flights connect.

> NOTE&nbsp; There is a representation of slabs for structural analysis provided by a proper subtype of _IfcStructuralMember_ being part of the _IfcStructuralAnalysisModel_.

> NOTE&nbsp; An arbitrary planar element to which this semantic information is not applicable or irrelevant shall be modeled as _IfcPlate_.

There are two main representations for slab occurrences:

* _IfcSlab_ with _IfcMaterialLayerSetUsage_ is used for all occurrences of slabs, that are prismatic and where the thickness parameter can be fully described by the _IfcMaterialLayerSetUsage_. These slabs are always represented geometrically by a 'SweptSolid' geometry (or by a 'Clipping' geometry based on 'SweptSolid'), if a 3D geometric representation is assigned. 
>> NOTE&nbsp; The entity _IfcSlabStandardCase_ has been deprecated, _IfcSlab_ with _IfcMaterialLayerSetUsage_ is used instead. 
* _IfcSlab_ without _IfcMaterialLayerSetUsage_ is used for all other occurrences of slabs, particularly for slabs with changing thickness, or slabs with non planar surfaces, and slabs having only 'SweptSolid' or 'Brep' geometry, or if a more parametric representation is not intended.

> NOTE&nbsp; The entity _IfcSlabElementedCase_ has been deprecated, _IfcSlab>_ with _IfcRelAggregates_ is used to describe occurrences of slabs which are aggregated from subordinate elements,.

> HISTORY&nbsp; New entity in IFC2.0; it is a merger of the two previous entities IfcFloor, IfcRoofSlab, introduced in IFC1.0