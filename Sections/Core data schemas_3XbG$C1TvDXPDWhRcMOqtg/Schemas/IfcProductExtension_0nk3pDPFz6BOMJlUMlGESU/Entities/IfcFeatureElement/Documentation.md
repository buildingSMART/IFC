A feature element is a generalization of all existence dependent elements which modify the shape and appearance of the associated master element. The _IfcFeatureElement_ offers the ability to handle shape modifiers as semantic objects within the IFC object model.

> NOTE&nbsp; The term "feature" has a predefined meaning in a context of "feature-based modeling" and within steel construction work. It is introduced here in a broader sense to cover all existence dependent, but semantically described, modifiers of an element's shape and appearance. It is envisioned that future releases enhance the feature-based capabilities of the IFC model.

In contrary to the aggregation, as used in _IfcElementAssembly_, that defines the aggregate as a container element, that has equally treated parts, the feature concept introduced by _IfcFeatureElement_ defines the master element with subordinate parts as additions, or with voids or cut-outs as subtractions.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x2}
> IFC2x2 CHANGE&nbsp; The entity is introduced as an upward compatible extension of the IFC2x platform. It is an intermediate abstract supertype without defining its own explicit attributes.