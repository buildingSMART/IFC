The following additional constraints apply to the 'AdvancedSweptSolid' representation type:

* **Solid**: _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported.
* **Solid Position** : The _IfcSweptAreaSolid.Position_ shall exclusively been used to correspond to the cardinal point. The x/y offset of the _Position_ represents the cardinal point offset of the profile against the axis. No rotation shall be allowed.
* **Profile**: all subtypes of _IfcProfileDef_ (with exception of _IfcArbitraryOpenProfileDef_)
* **Profile Position** : For all single profiles, the _IfcParameterizedProfileDef.Position_ shall be NIL, or having _Location_ = 0.,0. and _RefDirection_ = 1.,0.

> NOTE&nbsp; Using _IfcExtrudedAreaSolidTapered_, or _IfcRevolvedAreaSolidTapered_ requires the use of two _IfcMaterialProfile_'s within the _IfcMaterialProfileSetUsageTapering_ assinged to the _IfcBeamStandardCase_