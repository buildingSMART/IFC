The material of the _IfcWindow_ is defined by the _IfcMaterialConstituentSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial__.
It is accessible by the inverse _HasAssociations_ relationship. The following keywords for _IfcMaterialConstituentSet.MaterialConstituents[n].Name_ shall be used:_

* 'Lining' - to indicate that the material constituent applies to to the window lining
* 'Framing' - to indicate that the material constituent applies to to the window panels, if not provided, the 'Lining' material information applied to panels as well
* 'Glazing' - to indicate that the material constituent applies to to the glazing part

If the fall back single _IfcMaterial_ is referenced, it applies to the lining and framing of the window.