<An _IfcColumn_ is a vertical structural member which often is aligned with a structural grid intersection. It represents a vertical, or nearly vertical, structural member that transmits, through compression, the weight of the structure above to other structural elements below. It represents such a member from an architectural point of view. It is not required to be load bearing.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1  
> structural member of slender form, usually vertical, that transmits to its base the forces, primarily in compression, that are applied to it.

> NOTE&nbsp; The representation of a column in a structural analysis model is provided by _IfcStructuralCurveMember_ being part of an _IfcStructuralAnalysisModel_.

> NOTE&nbsp; For any longitudial structural member, not constrained to be predominately horizontal nor vertical, or where this semantic information is irrelevant, the entity _IfcMember_ exists.

There are two main representations for column occurrences:

* _IfcColumn_ with _IfcMaterialProfileSetUsage_ is used for all occurrences of columns, that have a profile defined that is swept along a directrix. The profile might be changed uniformly by a taper definition along the directrix. The profile parameter and its cardinal point of insertion can be fully described by the _IfcMaterialProfileSetUsage_. These columns are always represented geometricly by an 'Axis' and a 'SweptSolid' or 'AdvancedSweptSolid' shape representation (or by a 'Clipping' geometry based on the swept solid), if a 3D geometric representation is assigned. 
>> NOTE&nbsp; The entity _IfcColumnStandardCase_ has been deprecated, _IfcColumn_ with _IfcMaterialProfileSetUsage_ is used instead. 
* _IfcColumn_ is used for all other occurrences of columns, particularly for columns with changing profile sizes along the extrusion, or columns defined by non-linear extrusion, or columns having only 'Brep', or 'SurfaceModel' geometry, or if a more parametric representation is not intended.

> HISTORY&nbsp; New entity in IFC1.0