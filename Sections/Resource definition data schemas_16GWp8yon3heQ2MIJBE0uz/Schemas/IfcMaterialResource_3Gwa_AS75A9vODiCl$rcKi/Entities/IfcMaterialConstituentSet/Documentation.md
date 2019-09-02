_IfcMaterialConstituentSet_ is a collection of individual material constituents, each assigning a material to a part of an element. The parts are only identified by a keyword (as opposed to an _IfcMaterialLayerSet_ or _IfcMaterialProfileSet_ where each part has an individual shape parameter (layer thickness or layer profile).

> EXAMPLE The different materials of a window construction shall be provided for the window lining and the window glazing. An _IfcMaterialConstituentSet_ is assigned to the window with two _IfcMaterialConstituent_'s, one with the _Name_ = 'Lining', one with the _Name_ = 'Glazing'.

> NOTE&nbsp; See the "Material Use Definition" at the individual element to which an _IfcMaterialConstituentSet_ may apply for a required or recommended definition of such keywords.

> HISTORY New entity in IFC4.