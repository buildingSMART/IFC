Element assemblies may be used for compositions of parts used in other building elements, such as framing for walls and slabs.

Grids may be used to indicate coordinated placement, where _IfcGridAxis_ may use _IfcLine_ with an _IfcVector_ having a discrete magnitude to indicate a repetition interval; if such magnitude is defined, then any elements placed according to such grid axis implicitly repeat at the defined interval within the boundary defined at the occurrence ('Axis' representation for linear elements such as walls, 'FootPrint' representation for area-based elements such as slabs, 'BoundingBox' representation for volume-based elements such as cabinetry).

Figure 1 illustrates an element assembly type used for slab framing.

!["voiding"](../../../figures/ifcelementassemblytype-beamgrid.png "Figure 1 &mdash; Element assembly for slab framing")

Figure 2 illustrates an element assembly type used for wall framing.

!["voiding"](../../../figures/ifcelementassemblytype-bracedframe.png "Figure 2 &mdash; Element assembly for wall framing")