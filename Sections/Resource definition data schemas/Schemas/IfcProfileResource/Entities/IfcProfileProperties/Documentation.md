This is a collection of properties applicable to section profile definitions.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Entity made non-abstract. Subtypes _IfcGeneralProfileProperties_, _IfcStructuralProfileProperties_, and _IfcStructuralSteelProfileProperties_ deleted. Attribute _ProfileName_ deleted, use _ProfileDefinition.ProfileName_ instead. Attribute _ProfileDefinition_ made mandatory. Attributes _Name_, _Description_, and _HasProperties_ added (inherited from _IfcExtendedProperties_).

{ .use-head}
Property use definitions

The following sets of material property definitions are part of this IFC release. They are direct instantiations of _IfcProperties_ with the _Name_ attribute holding the property set name.

* [Pset_ProfileMechanical](../../psd/ifcprofileresource/Pset_ProfileMechanical.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
* [Pset_ProfileArbitraryHollowCore](../../psd/ifcprofileresource/Pset_ProfileArbitraryHollowCore.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))
* [Pset_ProfileArbitraryDoubleT](../../psd/ifcprofileresource/Pset_ProfileArbitraryDoubleT.xml) ([occurrence driven](../../ifckernel/lexical/ifcpropertysettemplatetypeenum.htm))

Figure 1 illustrates properties of _Pset_ProfileMechanical_.

<table>
<tr><td><image src="../../../../../../figures/ifcprofileproperties_mechanical.png" alt="Mechanical profile properties"></image></td></tr>
<tr><td><p class="figure">Figure 1 &mdash; Mechanical profile properties</p></td></tr>
</table>

Figure 2 illustrates properties of _Pset_Profile_ArbitraryDoubleT_.

<table>
<tr><td><image src="../../../../../../figures/ifcprofileproperties_double_t.png" alt="Double T profile properties"></image></td></tr>
<tr><td><p class="figure">Figure 2 &mdash; Hollow core profile properties</p></td></tr>
</table>

Figure 3 illustrates properties of _Pset_Profile_ArbitraryHollowCore_.

<table>
<tr><td><image src="../../../../../../figures/ifcprofileproperties_hollow_core.png" alt="Hollow core profile properties"></image></td></tr>
<tr><td><p class="figure">Figure 3 &mdash; Double T profile properties</p></td></tr>
</table>
