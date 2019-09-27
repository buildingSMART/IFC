﻿An _IfcPropertyDependencyRelationship_ describes an identified dependency between the value of one property and that of another.

> HISTORY&nbsp; New entity in IFC2x2

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Made subtype of _IfcResourceLevelRelationship_ (attribute order changed).

{ .use-head}
Use Definition

Whilst the _IfcPropertyDependencyRelationship_ may be used to describe the dependency, and it may do so in terms of the expression of how the dependency operates, it is not possible through the current IFC model for the value of the related property to be actually derived from the value of the relating property. The determination of value according to the dependency is required to be performed by an application that can then use the Expression attribute to flag the form of the dependency.
