The material of the _IfcDoor_ is defined by the _IfcMaterialConstituentSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_ relationship. It is accessible by the inverse _HasAssociations_ relationship.

The following keywords for _IfcMaterialConstituentSet.MaterialConstituents[n].Name_ shall be used:

* 'Lining' - to indicate that the material constituent applies to to the door lining
* 'Framing' - to indicate that the material constituent applies to to the door framing, if not provided, the 'Lining' material information applied to frams as well
* 'Glazing' - to indicate that the material constituent applies to to the glazing as well

If the fall back single _IfcMaterial_ is referenced, it applies to the lining and framing of the door.