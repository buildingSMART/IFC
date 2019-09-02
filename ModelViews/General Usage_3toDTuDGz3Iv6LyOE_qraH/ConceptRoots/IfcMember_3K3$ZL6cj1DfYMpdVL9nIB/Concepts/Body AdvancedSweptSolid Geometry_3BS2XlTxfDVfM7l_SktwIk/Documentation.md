The following constraints apply to the 'AdvancedSweptSolid' representation type:

* **Solid**: _IfcSurfaceCurveSweptAreaSolid_, _IfcFixedReferenceSweptAreaSolid_, _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported. 
>> NOTE&nbsp; View definitions and implementer agreements can further constrain the allowed swept solid types. 
* **Profile**: see 'SweptSolid' geometric representation
* **Extrusion**: not applicable

The following additional constraints apply to the 'AdvancedSweptSolid' representation type, when an _IfcMaterialProfileSetUsage_ is assigned to the _IfcMember_:

* **Solid**: _IfcSurfaceCurveSweptAreaSolid_, _IfcFixedReferenceSweptAreaSolid_, _IfcExtrudedAreaSolidTapered_, _IfcRevolvedAreaSolidTapered_ shall be supported. 
>> NOTE&nbsp; View definitions and implementer agreement can further constrain the allowed swept solid types. 
>> NOTE&nbsp; Using _IfcExtrudedAreaSolidTapered_, or _IfcRevolvedAreaSolidTapered_ requires the use of two _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ assinged to the _IfcBeamStandardCase_ 
* **Profile**: see 'SweptSolid' geometric representation
* **Profile Position** : see 'SweptSolid' geometric representation
* **Extrusion**: not applicable