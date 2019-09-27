﻿An _IfcSweptDiskSolid_ represents the 3D shape by a sweeping representation scheme allowing a two dimensional circularly bounded plane to sweep along a three dimensional _Directrix_ through space.

The _StartParam_ and _EndParam_ parameter are optional, if not provided they default to the start and end of the _Directrix_. Only if the _Directrix_ is given by a bounded or by a closed curve, it is permissible to omit the values of _StartParam_ and _EndParam_.

If the transitions between consecutive segments of the _Directrix_ are not tangent continuous, the resulting solid is created by a miter at half angle between the two segments. Informal proposition restricts the permissible angle between two non-tangent continuous segments.

Figure 1 illustrates an example.

* _Directrix_ given as _IfcIndexedPolyCurve_, having linear and circular arc segments, that are tangent continuous between each segments
* _Directrix_ being a bounded and open curve
* No _StartParam_ and _EndParam_ are provided, start and end default to start and end of the bounded curve of the _Directrix_

> NOTE&nbsp; Although the example shows a _Directrix_ as a poly curve on a planar reference surface, the definition of _IfcSweptDiskSolid_ is not restricted to be based on planer curves. However view definitions or implementer agreements may provide restrictions.

> NOTE&nbsp; The geometric item _IfcIndexedPolyCurve_ provides a more compact representation compared with _IfcCompositeCurve_ as is therefore the prefered curve representation for the _Directrix_.

!["disk solid"](../../../../../../figures/ifcsweptdisksolid-layout1.png "Figure 1 &mdash; Swept disk solid geometry")

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> A swept disk solid is the solid produced by sweeping a circular disk along a three dimensional curve. During the sweeping operation the normal to the plane of the circular disk is in the direction of the tangent to the directrix curve and the center of the disk lies on the directrix. The circular disk may, optionally, have a central hole, in this case the resulting solid has a through hole, or, an internal void when the directrix forms a close curve.

> NOTE&nbsp; Entity adapted from **swept_disk_solid** defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The attribute _StartParam_ and _EndParam_ have been made optional.

{ .spec-head}
Informal Propositions:

1. If the _Directrix_ curve definition is not tangent continuous, the transition between the segments has to be within an acceptable limit of tangent discontinuity. Very sharp edges may result in nearly impossible miter. Implementer agreements may define acceptable limits for tangent discontinuity.
2. The segments of the _Directrix_ shall be long enough to apply the _Radius_. In case of an arc segment forming part of the _Directrix_, its radius shall be greater then the disk _Radius_
3. The _Directrix_ shall not be based on an intersecting curve.
