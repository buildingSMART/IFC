An _IfcBeam_ is a horizontal, or nearly horizontal, structural member that is capable of withstanding load primarily by resisting bending. It represents such a member from an architectural point of view. It is not required to be load bearing.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1: structural member for carrying load(s) between or beyond points of support, usually narrow in relation to its length and horizontal or nearly so.

> NOTE&nbsp; The representation of load-bearing beams in a structural analysis model is provided by subtypes of _IfcStructuralMember_ (with _IfcStructuralCurveMember_ being mostly applicable) as part of an _IfcStructuralAnalysisModel_.

> NOTE&nbsp; For any other longitudinal structural member, not constrained to be predominately horizontal nor vertical, or where this semantic information is irrelevant, the entity _IfcMember_ should be used.

There are two main representations for beam occurrences:

* _IfcBeam_ with _IfcMaterialProfileSetUsage_ is used for all occurrences of beams, that have a profile defined that is swept along a directrix. The profile might be changed uniformly by a taper definition along the directrix. The profile parameter and its cardinal point of insertion can be fully described by the _IfcMaterialProfileSetUsage_. These beams are always represented geometricly by an 'Axis' and a 'SweptSolid' or 'AdvancedSweptSolid' shape representation (or by a 'Clipping' geometry based on the swept solid), if a 3D geometric representation is assigned. 
>> NOTE&nbsp; The entity _IfcBeamStandardCase_ has been deprecated, _IfcBeam_ with _IfcMaterialProfileSetUsage_ is used instead. 
* _IfcBeam_ without _IfcMaterialProfileSetUsage_ is used for all other occurrences of beams, particularly for beams with non-uniformly changing profile sizes along the sweep, or beams having only 'AdvancedBrep', 'Brep', or 'SurfaceModel' geometry, or if a more parametric representation is not intended.

> HISTORY&nbsp; New entity in IFC1.0