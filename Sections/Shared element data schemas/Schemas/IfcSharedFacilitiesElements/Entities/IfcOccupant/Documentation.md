An occupant is a type of actor that defines the form of occupancy of a property.

The principal purpose of **IfcOccupant** is to determine the nature of occupancy of a property for a particular actor. All characteristics relating to the actor (name and organization details) are inherited from the _IfcActor_ entity.

> HISTORY&nbsp; New entity in IFC2x

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcActor_: [Property Sets for Objects](../../templates/property-sets-for-objects.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcoccupant.htm)

{ .use-head}
Actor Assignment

The [Actor Assignment](../../templates/actor-assignment.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcspatialstructureelement.htm">IfcSpatialStructureElement</a></td><td>Indicates the property to be occupied. Particular details of the agreement relating to the occupancy of a property are dealt within the <em>Pset_PropertyAgreement</em> that is defined for the instance of <em>IfcSpatialStructureElement</em>. This means that an occupant may be related to a site, building, building storey or space through the <em>IfcSpatialStructureElement.ElementComposition</em> attribute. For instance, if the property concerned is several office spaces on a building storey, it might be appropriate to reference <em>IfcBuildingStorey.ElementComposition=PARTIAL</em>.  Occupants of a property may be considered to be the parties to an agreement. The roles that the occupant may play in respect to an agreement are defined in the <em>IfcOccupantTypeEnum</em> enumeration. If the role is not specified by the predefined contents of this enumeration, the value <em>USERDEFINED</em> may be set and the <em>ObjectType</em> attribute asserted.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifccontrol.htm">IfcControl</a></td><td>Indicates project directives issued by the actor.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcgroup.htm">IfcGroup</a></td><td>Indicates groups for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcproduct.htm">IfcProduct</a></td><td>Indicates products for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcprocess.htm">IfcProcess</a></td><td>Indicates processes for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcresource.htm">IfcResource</a></td><td>Indicates resources for which the actor is responsible.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcOccupant Actor Assignment</p></td></tr></table>