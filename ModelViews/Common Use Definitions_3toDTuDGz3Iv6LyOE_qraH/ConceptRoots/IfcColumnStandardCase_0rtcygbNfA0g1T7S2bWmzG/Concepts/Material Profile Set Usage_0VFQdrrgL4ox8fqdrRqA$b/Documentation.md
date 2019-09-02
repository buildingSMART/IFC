The _IfcColumnStandardCase_ defines in addition that the _IfcColumnType_ should have a unique _IfcMaterialProfileSet_, that is referenced by the _IfcMaterialProfileSetUsage_ assigned to all occurrences of this _IfcColumnType_. Composite profile columns can be represented by refering to several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ that is referenced from the _IfcMaterialProfileSetUsage_.

Figure 1 illustrates assignment of _IfcMaterialProfileSetUsage_ and _IfcMaterialProfileSet_ to the _IfcColumnStandardCase_ as the column occurrence and to the _IfcColumnType_. The same _IfcMaterialProfileSet_ shall be shared by many occurrences of _IfcMaterialProfileSetUsage_. This relationship shall be consistent to the relationship between the _IfcColumnType_ and the _IfcColumnStandardCase_.

!["Material profile set and usage"](../../../figures/IfcColumnStandardCase-01.png "Figure 1 &mdash; Column profile usage")

Figure 2 illustrates cardinal point alignment.

> NOTE  It has to be guaranteed that the use of _IfcCardinalPointEnum_ is consistent to the placement of the extrusion body provided by _IfcExtrudedAreaSolid.Position_

> NOTE  The cardinal points **7** (top left), and **6** (mid-depth right) are assigned according to the definition at _IfcCardinalPointReference_

!["Cardinal point usage"](../../../figures/IfcColumnStandardCase_CardinalPoint.png "Figure 2 &mdash; Column cardinal points")

Figure 3 illustrates assignment of a composite profile by using _IfcCompositeProfile_ for geometric representation and several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_. The number of _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ is restricted to maximal 2 and requires the use of _IfcExtrudedAreaSolidTapered_, or _IfcRevolvedAreaSolidTapered_ for the correct 'Body' shape representation.

!["Material profile set and usage"](../../../figures/IfcColumnStandardCase-02.png "Figure 3 &mdash; Column composite profiles")