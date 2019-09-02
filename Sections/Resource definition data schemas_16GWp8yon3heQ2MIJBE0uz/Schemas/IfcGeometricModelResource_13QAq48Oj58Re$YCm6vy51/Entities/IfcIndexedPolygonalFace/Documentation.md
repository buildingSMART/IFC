The _IfcIndexedPolygonalFace_ is a compact representation of a planar face being part of a face set. The vertices of the polygonal planar face are provided by 3 or more Cartesian points, defined by indices that point into an _IfcCartesianPointList3D_, either direcly, or via the _PnIndex_, if provided at _IfcPolygonalFaceSet_.

Figure 1 shows an _IfcIndexedPolygonalFace_ at an _IfcPolygonalFaceSet_ not using _PnIndex_ (the default).

!["IfcIndexedPolygonalFace"](../../../figures/ifcindexedpolygonalface_01.png "Figure 1 &mdash; Polygonal face geometry provided by indices into a point list")

&nbsp;

Figure 2 shows an _IfcIndexedPolygonalFace_ at an _IfcPolygonalFaceSet_ using _PnIndex_.

!["IfcIndexedPolygonalFace us
ing PnIndex"](../../../figures/ifcindexedpolygonalface_02.png "Figure 2 &mdash; Polygonal face geometry provided by indices into a point list")

> HISTORY&nbsp; New entity in IFC4 Addendum 2.