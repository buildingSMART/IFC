The _IfcCostResource_ schema provides the means to identify cost and environmental impact values that may be assigned to an object.

### Applied Value
An applied value is either a cost or an environmental impact value that specifies an amount or a value that has an effect on the amount that is applied to an object in the units of measure applicable to the value type. An applied value may have an applicable date. In the case of a cost, that can be used to provide a basis on which fluctuations in price can be established or that otherwise identifies when the cost value was applied.

Each applied value may have a unit basis which determines how a total value should be determined for objects. This is relevant where values are identified per unit quantity of an item.

### Applied Value Relationship
An individual applied value may be defined according to the values of a set of component values and may also be identified as a component of other values. This is achieved through the assertion of an applied value relationship which acts as a container for applied value components.

### Referencing Value Documents
The origin of an applied value may be a documentary source. The _IfcCostResource_ schema allows identification of such a source through a document reference. _IfcReferencesValueDocument_ is a relationship class that allows many instances of _IfcAppliedValue_ to be referenced from a single such document.