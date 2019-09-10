_IfcRoot_ is the most abstract and root class for all IFC entity definitions that roots in the kernel or in subsequent layers of the IFC object model. It is therefore the common supertype of all IFC entities, beside those defined in an IFC resource schema. All entities that are subtypes of _IfcRoot_ can be used independently, whereas resource schema entities, that are not subtypes of _IfcRoot_, are not supposed to be independent entities.

> NOTE&nbsp; View definitions and implementation agreement may impose additional restrictions on the use of the _OwnerHistory_ to handle object versioning.

> HISTORY&nbsp; New entity in IFC1.0

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The attribute _OwnerHistory_ has been made OPTIONAL.

___
## Common Use Definitions
[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcroot.htm)

{ .use-head}
Identity

The [Identity](../../templates/identity.htm) concept applies to this entity.

_IfcRoot_ assigns the globally unique ID. In addition it may provide for a name and a description about the concept.

  
  
{ .use-head}
Revision Control

The [Revision Control](../../templates/revision-control.htm) concept applies to this entity.

Ownership, history, and merge state is captured using _IfcOwnerHistory_.
