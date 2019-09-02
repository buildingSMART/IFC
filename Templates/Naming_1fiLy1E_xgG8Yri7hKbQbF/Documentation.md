Provision of basic element attributes for the _element_. It includes:

*  _Name_
*  _Description_
*  _PredefinedType_(if available at the element entity definition) as ,
*  _ObjectType being the_<span style="font-style: italic;">u</span>ser defined type, if the _PredefinedType_ is set to USERDEFINED.

Additionally all subtypes of _IfcSpatialStructureElement_, _IfcSite_, _IfcBuilding_, IfcBuildingStorey, and _IfcSpace_add an additional attribute, _LongName_.

This information is provided as direct attributes at the _element_. The default requirement stipulated by this **concept template** is that the provision of a _Name_and of a _PredefinedType_(if available) is mandatory, whereas the provision of a _Description_and an _ObjectType_is optional.

A **model view definitio**n shall clearly define which of those attributes are required to have values, and if there are constraints on those values.