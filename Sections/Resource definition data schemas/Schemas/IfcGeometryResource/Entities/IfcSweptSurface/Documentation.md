﻿An _IfcSweptSurface_ is a surface defined by sweeping a curve. The swept surface is defined by a open or closed curve, represented by a subtype if _IfcProfileDef_, that is provided as a two-dimensional curve on an implicit plane, and by the sweeping operation.

* The swept curve is defined by positioning the profile in the xy plane of the object coordinate system, 
* The sweeping operation is applied to the swept curve as defined within the subtypes of _IfcSweptSurface_;

The optional _Positio_n coordinate system allows for re-positioning the resulting swept surface relative to the object coordinate system.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> A swept surface is one that is constructed by sweeping a curve along another curve.

> NOTE&nbsp; Entity adapted from **swept_surface** defined in ISO 10303-42.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The attribute _Position_ has been changed to OPTIONAL with upward compatibility for file-based exchange.
