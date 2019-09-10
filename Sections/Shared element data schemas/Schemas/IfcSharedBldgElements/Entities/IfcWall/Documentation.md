The wall represents a vertical construction that bounds or subdivides spaces. Wall are usually vertical, or nearly vertical, planar elements, often designed to bear structural loads. A wall is however not required to be load bearing.

{ .extDef}
> NOTE&nbsp; Definition according to ISO 6707-1: vertical construction usually in masonry or in concrete which bounds or subdivides a construction works and fulfils a load bearing or retaining function.

> NOTE&nbsp; There is a representation of walls for structural analysis provided by a proper subtype of _IfcStructuralMember_ being part of the _IfcStructuralAnalysisModel_.

> NOTE&nbsp; An arbitrary planar element to which this semantic information is not applicable (is not predominantly vertical), shall be modeled as _IfcPlate_.

There are two main representations for for wall occurrences:

* _IfcWall_ with _IfcMaterialLayerSetUsage_ is used for all occurrences of walls, that have a non-changing thickness along the wall path and where the thickness parameter can be fully described by a material layer set. These walls are always represented geometrically by an 'Axis' and a 'SweptSolid' shape representation (or by a 'Clipping' geometry based on 'SweptSolid'), if a 3D geometric representation is assigned. 
>> NOTE&nbsp; The entity _IfcWallStandardCase_ has been deprecated, _IfcWall_ with _IfcMaterialLayerSetUsage_ is used instead. 
* _IfcWall_ without _IfcMaterialLayerSetUsage_ is used for all other occurrences of wall, particularly for walls with changing thickness along the wall path (e.g. polygonal walls), or walls with a non-rectangular cross sections (e.g. L-shaped retaining walls), and walls having an extrusion axis that is unequal to the global Z axis of the project (i.e. non-vertical walls), or walls having only 'Brep', or 'SurfaceModel' geometry, or if a more parametric representation is not intended.

> NOTE&nbsp; The entity _IfcWallbElementedCase_ has been deprecated, _IfcWall>_ with _IfcRelAggregates_ is used to describe occurrences of wall which are aggregated from subordinate elements, such as wall panels.

> HISTORY&nbsp; New entity in IFC1.0
