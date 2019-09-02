The following additional constraints apply to the 'AdvancedSweptSolid' representation type:

* **Solid**: _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported. 
* **Profile**: all subtypes of _IfcProfileDef_ (with exception of _IfcArbitraryOpenProfileDef_)
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.

> NOTE&nbsp; Using _IfcExtrudedAreaSolidTapered_, or _IfcRevolvedAreaSolidTapered_ requires the use of two _IfcMaterialProfile_'s within the _IfcMaterialProfileSetUsageTapering_ assinged to the _IfcColumnStandardCase_