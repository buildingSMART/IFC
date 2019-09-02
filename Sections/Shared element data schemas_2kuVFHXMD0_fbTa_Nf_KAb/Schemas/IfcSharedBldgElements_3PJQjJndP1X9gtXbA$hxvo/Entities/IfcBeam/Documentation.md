An _IfcBeam_ is a horizontal, or nearly horizontal, structural member that is capable of withstanding load primarily by resisting bending. It represents such a member from an architectural point of view. It is not required to be load bearing.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1: structural member for carrying load(s) between or beyond points of support, usually narrow in relation to its length and horizontal or nearly so.

> NOTE&nbsp; The representation of load-bearing beams in a structural analysis model is provided by subtypes of _IfcStructuralMember_ (with _IfcStructuralCurveMember_ being mostly applicable) as part of an _IfcStructuralAnalysisModel_.

> NOTE&nbsp; For any other longitudinal structural member, not constrained to be predominately horizontal nor vertical, or where this semantic information is irrelevant, the entity _IfcMember_ should be used.

There are two entities for beam occurrences:

* _IfcBeamStandardCase_ used for all occurrences of beams, that have a profile defined that is swept along a directrix. The profile might be changed uniformly by a taper definition along the directrix. The profile parameter and its cardinal point of insertion can be fully described by the _IfcMaterialProfileSetUsage_. These beams are always represented geometricly by an 'Axis' and a 'SweptSolid' or 'AdvancedSweptSolid' shape representation (or by a 'Clipping' geometry based on the swept solid), if a 3D geometric representation is assigned. In addition they have to have a corresponding _IfcMaterialProfileSetUsage_ assigned. 
>> NOTE&nbsp; Model view definitions and implementer agreements may further constrain the applicable geometry types, for example, by excluding tapering from an _IfcBeamStandardCase_ implementation. 
* _IfcBeam_ used for all other occurrences of beams, particularly for beams with changing profile sizes along the extrusion, or beams defined by non-linear extrusion, or beams having only 'Brep', or 'SurfaceModel' geometry. 
>> NOTE&nbsp; Model view definitions and implementer agreements may impose the use of _IfcBeam_ in all cases by excluding _IfcBeamStandardCase_ from scope of the model view. 
    * _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
    * _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
    * _IfcBuildingElement_: [Surface 3D Geometry](../../templates/surface-3d-geometry.htm)

    * the _Spatial Containment_ (defined here), or
    * the _Element Composition_.

    * **Solid**: _IfcExtrudedAreaSolid_, _IfcRevolvedAreaSolid_ shall be supported
    * **Profile**: all subtypes of _IfcProfileDef_ (with exception of _IfcArbitraryOpenProfileDef_)
    * **Extrusion**:&nbsp; All extrusion directions shall be supported.

    * **Solid**: _IfcSurfaceCurveSweptAreaSolid_, _IfcFixedReferenceSweptAreaSolid_, _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported. 
>>> NOTE&nbsp; View definitions and implementer agreement can further constrain the allowed swept solid types. 
    * **Profile**: see 'SweptSolid' geometric representation
    * **Extrusion**: not applicable

    * **Solid**: see 'SweptSolid' geometric representation
    * **Profile**: see 'SweptSolid' geometric representation
    * **Extrusion**: see 'SweptSolid' geometric representation
    * **Boolean result**: The _IfcBooleanClippingResult_ shall be supported, allowing for Boolean differences between the swept solid (here _IfcExtrudedAreaSolid_) and one or several _IfcHalfSpaceSolid_ (or its subtypes).