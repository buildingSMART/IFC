The survey point representation of _IfcSite_ is defined using a set of survey points and optionally breaklines. The breaklines are restricted to only connect points given in the set of survey points. Breaklines, if given, are used to constrain the triangulation.

The representation identifier and type of this geometric representation of _IfcSite_ is:

* _IfcShapeRepresentation.RepresentationIdentifier_ = 'SurveyPoints'
* _IfcShapeRepresentation.RepresentationType_ = 'GeometricCurveSet'

Figure 1 shows a set of survey points, given as 3D Cartesian points within the object coordinate system of the site. Figure 2 shows the result after facetation.

The set of _IfcCartesianPoint_ is included in the set of _IfcGeometricCurveSet.Elements_.

<table cellpadding="2" cellspacing="2" summary="survey points representation">
<tr>
<td><img src="../../../figures/IfcSite-Standard-points.gif" alt="points only" border="0" height="300" width="400"></td>
<td><img src="../../../figures/IfcSite-Standard-facets-points.gif" alt="facetation of points" border="0" height="300" width="400"></td>
</tr>
<tr>
<td width="400"><p class="figure">Figure 1 &mdash; Site survey points</p></td>
<td width="400"><p class="figure">Figure 2 &mdash; Site survey points facetation</p></td>
</tr>
</table>

Figure 3 shows A set of survey points, given as 3D Cartesian points, and a set of break points, given as a set of lines, connecting some survey points, within the object coordinate system of the site. Figure 4 shows the result after facetation.

The set of _IfcCartesianPoint_ and the set of _IfcPolyline_ are included in the set of _IfcGeometricCurveSet.Elements_.

<table cellpadding="2" cellspacing="2" summary="survey points representation">
<tr>
<td><img src="../../../figures/IfcSite-Standard-breaklines.gif" alt="breaklines" border="0" height="300" width="400"></td>
<td><img src="../../../figures/IfcSite-Standard-facets-breaklines.gif" alt="facetation with breakpoints" border="0" height="300" width="400"></td>
</tr>
<tr>
<td width="400"><p class="figure">Figure 3 &mdash; Site breaklines</p></td>
<td width="400"><p class="figure">Figure 4 &mdash; Site breaklines facetation</p></td>
</tr>
</table>

> NOTE&nbsp; The geometric representation of the site has been based on the ARM level description of the site_shape_representation given within the ISO 10303-225 "Building Elements using explicit shape representation".