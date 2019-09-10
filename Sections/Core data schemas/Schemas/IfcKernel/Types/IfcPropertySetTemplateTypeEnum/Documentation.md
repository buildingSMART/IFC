This enumeration defines the general applicability of instances of _IfcPropertySet_, or _IfcElementQuantity_ defined by this _IfcPropertySetTemplate_, to subtypes of _IfcObjectDefinition_.

> HISTORY&nbsp; New enumeration in IFC4.

{ .spec-head}
Enumerated Item Definitions:

* **PSET_TYPEDRIVENONLY**: the property sets defined by this _IfcPropertySetTemplate_ can only be assigned to subtypes of _IfcTypeObject_.
* **PSET_TYPEDRIVENOVERRIDE**: the property sets defined by this _IfcPropertySetTemplate_ can be assigned to subtypes of _IfcTypeObject_ and can be overridden by a property set with same name at subtypes of _IfcObject_.
* **PSET_OCCURRENCEDRIVEN**: the property sets defined by this _IfcPropertySetTemplate_ can only be assigned to subtypes of _IfcObject_.
* **PSET_PERFORMANCEDRIVEN**: the property sets defined by this _IfcPropertySetTemplate_ can only be assigned to _IfcPerformanceHistory_,
* **QTO_TYPEDRIVENONLY**: the element quantity defined by this _IfcPropertySetTemplate_ can only be assigned to subtypes of _IfcTypeObject_.
* **QTO_TYPEDRIVENOVERRIDE**: the element quantity defined by this _IfcPropertySetTemplate_ can be assigned to subtypes of _IfcTypeObject_ and can be overridden by an element quantity with same name at subtypes of _IfcObject_.
* **QTO_OCCURRENCEDRIVEN**: the element quantity defined by this _IfcPropertySetTemplate_ can only be assigned to subtypes of _IfcObject_.
* **NOTDEFINED**: No restriction provided, the property sets defined by this _IfcPropertySetTemplate_ can be assigned to any entity, if not otherwise restricted by the _ApplicableEntity_ attribute.
