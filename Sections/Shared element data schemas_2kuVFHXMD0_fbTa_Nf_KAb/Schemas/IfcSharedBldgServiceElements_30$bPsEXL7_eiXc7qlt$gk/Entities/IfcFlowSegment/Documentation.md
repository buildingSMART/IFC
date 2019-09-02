The distribution flow element _IfcFlowSegment_ defines the occurrence of a segment of a flow distribution system.

The _IfcFlowSegment_ defines a particular occurrence of a segment inserted in the spatial context of a project. The parameters defining the type of the segment and/or its shape are defined by the _IfcFlowSegmentType_, which is related by the inverse relationship IsDefinedBy pointing to _IfcRelDefinesByType_.

> HISTORY&nbsp; New entity in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; This entity has been deprecated for instantiation and will become ABSTRACT in a future release; new subtypes should now be used instead.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)
* _IfcDistributionElement_: [Quantity Sets](../../templates/quantity-sets.htm), [Spatial Containment](../../templates/spatial-containment.htm)
* _IfcDistributionFlowElement_: [Object Typing](../../templates/object-typing.htm), [Property Sets for Objects](../../templates/property-sets-for-objects.htm), [Clearance Geometry](../../templates/clearance-geometry.htm), [Lighting Geometry](../../templates/lighting-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcflowsegment.htm)

{ .use-head}
Material Profile Set Usage

The [Material Profile Set Usage](../../templates/material-profile-set-usage.htm) concept applies to this entity.

The material of the **IfcFlowSegment** is defined using one of the following entities:

* [IfcMaterialProfileSetUsage](../../ifcmaterialresource/lexical/ifcmaterialprofilesetusage.htm) : for parametric segments, this defines the cross section and alignment to the 'Axis' representation, from which the 'Body' representation may be generated.
* [IfcMaterialProfileSet](../../ifcmaterialresource/lexical/ifcmaterialprofilesetusage.htm) : for non-parametric segments (having fixed length or path), this may define the cross section for analysis purposes, however the 'Body' representation is independently generated.
* [IfcMaterialConstituentSet](../../ifcmaterialresource/lexical/ifcmaterialconstituentset.htm) : for elements containing multiple materials where profiles are not applicable, this indicates materials at named parts. 
*  [IfcMaterial](../../ifcmaterialresource/lexical/ifcmaterial.htm) : for elements comprised of a single material where profiles are not applicable, this indicates the material.

The material is attached by the _RelatingMaterial_ attribute on the [IfcRelAssociatesMaterial](../../ifcproductextension/lexical/ifcrelassociatesmaterial.htm) relationship. It is accessible by the _HasAssociations_ inverse attribute. Material information can also be given at the [IfcFlowSegmentType](../../ifcsharedbldgserviceelements/lexical/ifcflowsegmenttype.htm), defining the common attribute data for all occurrences of the same type. Standard names and material types are defined at subtypes.

  
  
{ .use-head}
Axis Geometry

The [Axis Geometry](../../templates/axis-geometry.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th></tr>
<tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcFlowSegment Axis Geometry</p></td></tr></table>

Standard representations are defined at the supertype _IfcDistributionFlowElement_. For parametric flow segments where [IfcMaterialProfileSetUsage](../../ifcmaterialresource/lexical/ifcmaterialprofilesetusage.htm) is defined and an 'Axis' representation is defined, then the 'Body' representation may be generated using the 'SweptSolid' or 'AdvancedSweptSolid' representation types by sweeping the profile(s) along the axis.