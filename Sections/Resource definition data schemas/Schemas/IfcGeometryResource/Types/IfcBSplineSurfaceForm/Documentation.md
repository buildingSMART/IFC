The _IfcBSplineSurfaceForm_ represents a part of a surface of some specific form.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> This type is used to indicate that the B-spline surface represents a part of a surface of some specific form.

> NOTE&nbsp; Type adapted from **b_spline_surface_form** defined in ISO 10303-42.

> HISTORY&nbsp; New type in IFC4.

{ .spec-head}
Enumerated Item Definitions:

* **plane_surf**: A bounded portion of a plane represented by a B-spline surface of degree 1 in each parameter.
* **cylindrical_surf**: A bounded portion of a cylindrical surface.
* **conical_surf**: A bounded portion of the surface of a right circular cone.
* **spherical_surf**: A bounded portion of a sphere, or a complete sphere, represented by a B-spline surface.
* **toroidal_surf**: A torus, or portion of a torus, represented by a B-spline surface.
* **surf_of_revolution**: A bounded portion of a surface of revolution.
* **ruled_surf**: A surface constructed from two parametric curves by joining with straight lines corresponding points with the same parameter value on each of the curves.
* **generalised_cone**: A special case of a ruled surface in which the second curve degenerates to a single point; when represented by a B-spline surface all the control points along one edge will be coincident.
* **quadric_surf**: A bounded portion of one of the class of surfaces of degree 2 in the variables x, y and z.
* **surf_of_linear_extrusion**: A bounded portion of a surface of linear extrusion represented by a B-spline surface of degree 1 in one of the parameters.
* **unspecified**: A surface for which no particular form is specified.
