{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> This function builds and returns three normalized orthogonal directions. u[3] is the direction of axis. u[1] is in the direction of the projection of ref_direction onto the plane normal to u[3] and u[2] is the cross product of u[3] and u[1]. Default values are supplied if input data is incomplete.

> NOTE&nbsp; Function adapted from **build_axes** defined in ISO 10303-42.

> HISTORY&nbsp; New function in IFC1.5