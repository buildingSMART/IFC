Figure 1 illustrates assignment of _IfcMaterialProfileSetUsage_ and _IfcMaterialProfileSet_ to the _IfcMember_ as the member occurrence and to the _IfcMemberType_. The same _IfcMaterialProfileSet_ shall be shared by many occurrences of _IfcMaterialProfileSetUsage_. This relationship shall be consistent to the relationship between the _IfcMemberType_ and the _IfcMember_.

!["Material profile set and usage"](../../../figures/ifcmemberstandardcase-01.png "Figure 1 &mdash; Member profile usage")

Figure 2 illustrates assignment of a composite profile by using _IfcCompositeProfile_ for geometric representation and several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_. The number of _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ is restricted to maximal 2 and requires the use of _IfcExtrudedAreaSolidTapered_, or _IfcRevolvedAreaSolidTapered_ for the correct 'Body' shape representation.

!["Material profile set and usage"](../../../figures/ifcmemberstandardcase-02.png "Figure 2 &mdash; Member composite profiles")

The material of the _IfcMember_ is defined by _IfcMaterialProfileSetUsage_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Composite profile members can be represented by refering to several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ that is referenced from the _IfcMaterialProfileSetUsage_.

Material information can also be given at the _IfcMemberType_, defining the common attribute data for all occurrences of the same type. It is then accessible by the inverse _IsDefinedBy_ relationship pointing to _IfcMemberType.HasAssociations_ and via _IfcRelAssociatesMaterial.RelatingMaterial_. See **Type Use
Definition** for additional agreements for standard members.