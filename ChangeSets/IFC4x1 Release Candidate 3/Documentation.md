Release Candidate 3 completes the alignment and geometry definitions for infrastructure. It is anticipated to be the final release candidate before the official publication of IFC 4.1.

A new general transition curve type _IfcTransitionCurveSegment2D_ may be used to define various transitions between straight segments and circular arcs, and deprecates _IfcClothoidalArcSegment2D_.

A new geometric curve type _IfcOffsetCurveByDistances_ may be used to define "string lines" having variable lateral and vertical offsets relative to a parent alignment curve, supporting super-elevations of roads and railways.

A new placement structure _IfcLinearPlacement_ enables physical and spatial objects to be positioned along alignment curves or derivate string line curves.

A new data structure _IfcCartesianPointList2DLabelled_ enables cross-sections to be defined where individual points are associated with string lines, to define geometry where the cross-section varies along an alignment.

A new geometric solid type _IfcSectionedSolidHorizontal_ may be used to define swept solids for road surfaces or bridge decks with control over the orientation of cross-sections.

A new tessellated geometry type _IfcTriangulatedIrregularNetwork_ may be used to efficiently define terrain surfaces with breaklines, holes, and voids.
