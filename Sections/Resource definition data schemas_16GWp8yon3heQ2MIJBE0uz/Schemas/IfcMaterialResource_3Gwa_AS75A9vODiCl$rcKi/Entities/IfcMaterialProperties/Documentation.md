The _IfcMaterialProperties_ assigns a set of material properties to associated material definitions. The set may be identified by a _Name_ and a _Description_. The _IfcProperty_ (instantiable subtypes) is used to express the individual material properties by name, description, value and unit.

> NOTE&nbsp; The set of material properties can be assigned to an individual _IfcMaterial_, a set or composite of materials (_IfcMaterialConstituent_, _IfcMaterialConstituentSet_), or set or individual material layer (_IfcMaterialLayer_, _IfcMaterialLayerSet_), or a set or individual material profile (_IfcMaterialProfile_, _IfcMaterialProfileSet_)

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Entity made non-abstract. The subtypes IfcMechanicalMaterialProperties, IfcThermalMaterialProperties, IfcHygroscopicMaterialProperties, IfcGeneralMaterialProperties, IfcOpticalMaterialProperties, IfcWaterProperties, IfcFuelProperties, IfcProductsOfCombustionProperties, IfcExtendedMaterialProperties have been deleted, use _IfcMaterialProperties_ instead.

&nbsp;

{ .use-head}
Property use definitions

The following sets of material property definitions are part of this IFC release. They are direct instantiations of _IfcProperties_ with the _Name_ attribute holding the property set name.

* **(All Types)** 
    * [Pset_MaterialCombustion](../../psd/ifcmaterialresource/Pset_MaterialCombustion.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialCommon](../../psd/ifcmaterialresource/Pset_MaterialCommon.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialEnergy](../../psd/ifcmaterialresource/Pset_MaterialEnergy.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialFuel](../../psd/ifcmaterialresource/Pset_MaterialFuel.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialHygroscopic](../../psd/ifcmaterialresource/Pset_MaterialHygroscopic.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialMechanical](../../psd/ifcmaterialresource/Pset_MaterialMechanical.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialOptical](../../psd/ifcmaterialresource/Pset_MaterialOptical.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialThermal](../../psd/ifcmaterialresource/Pset_MaterialThermal.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialWater](../../psd/ifcmaterialresource/Pset_MaterialWater.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm)) 
* **Concrete** 
    * [Pset_MaterialConcrete](../../psd/ifcmaterialresource/Pset_MaterialConcrete.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm)) 
* **Steel** 
    * [Pset_MaterialSteel](../../psd/ifcmaterialresource/Pset_MaterialSteel.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm)) 
* **Wood** 
    * [Pset_MaterialWood](../../psd/ifcmaterialresource/Pset_MaterialWood.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialWoodBasedBeam](../../psd/ifcmaterialresource/Pset_MaterialWoodBasedBeam.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
    * [Pset_MaterialWoodBasedPanel](../../psd/ifcmaterialresource/Pset_MaterialWoodBasedPanel.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))