﻿The _IfcMaterialProperties_ assigns a set of material properties to associated material definitions. The set may be identified by a _Name_ and a _Description_. The _IfcProperty_ (instantiable subtypes) is used to express the individual material properties by name, description, value and unit.

> NOTE&nbsp; The set of material properties can be assigned to an individual _IfcMaterial_, a set or composite of materials (_IfcMaterialConstituent_, _IfcMaterialConstituentSet_), or set or individual material layer (_IfcMaterialLayer_, _IfcMaterialLayerSet_), or a set or individual material profile (_IfcMaterialProfile_, _IfcMaterialProfileSet_)

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Entity made non-abstract. The subtypes IfcMechanicalMaterialProperties, IfcThermalMaterialProperties, IfcHygroscopicMaterialProperties, IfcGeneralMaterialProperties, IfcOpticalMaterialProperties, IfcWaterProperties, IfcFuelProperties, IfcProductsOfCombustionProperties, IfcExtendedMaterialProperties have been deleted, use _IfcMaterialProperties_ instead.

&nbsp;
