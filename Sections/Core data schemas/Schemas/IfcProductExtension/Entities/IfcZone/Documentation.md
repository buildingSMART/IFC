A zone is a group of spaces, partial spaces or other zones. Zone structures may not be hierarchical (in contrary to the spatial structure of a project - see _IfcSpatialStructureElement_), i.e. one individual _IfcSpace_ may be associated with zero, one, or several _IfcZone_'s. _IfcSpace_'s are grouped into an _IfcZone_ by using the objectified relationship _IfcRelAssignsToGroup_ as specified at the supertype _IfcGroup_.

> NOTE&nbsp; Certain use cases may restrict the freedom of non hierarchical relationships. In some building service use cases the zone denotes a view based delimited volume for the purpose of analysis and calculation. This type of zone cannot overlap with respect to that analysis, but may overlap otherwise.

> HISTORY&nbsp; New entity in IFC1.0

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The entity is now subtyped from _IfcSystem_ (not its supertype _IfcGroup_) with upward compatibility for file based exchange.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifczone.htm)

{ .use-head}
Object Classification

The [Object Classification](../../templates/object-classification.htm) concept applies to this entity.

Additional classifications of the _IfcZone_, as provided by a national classification system, can be assigned by using the _IfcRelAssociatesClassification_ relationship, accessible via the inverse attribute _HasAssociations_. The _IfcZone_ can be assigned to a spatial structure element, it refers to, e.g. to a particular _IfcBuildingStorey_ by using the _IfcRelServicesBuildings_ relationship, accessible via the inverse attribute _ServicesBuilding_.

  
  
{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_ZoneCommon.xml">Pset_ZoneCommon</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLifeFactors.xml">Pset_ServiceLifeFactors</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcZone Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Group Assignment

The [Group Assignment](../../templates/group-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcspatialstructureelement.htm">IfcSpatialStructureElement</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcZone Group Assignment</p></td></tr></table>

An _IfcZone_ is a spatial system under which individual _IfcSpace_'s (and other _IfcZone_'s) are grouped. In contrary to the _IfcSpatialZone_ entity, _IfcZone_ is a mere grouping, it can not define an own geometric representation and placement. Therefore it cannot be used for spatial zones having a different shape and size compared to the shape and size of aggregated spaces.

> NOTE&nbsp; The _IfcZone_ is regarded as the spatial system (as compared to the building service, electrical, or analytical system), the name remains _IfcZone_ for compatibility reasons, instead of using a proper naming convention, like IfcSpatialSystem.

> NOTE&nbsp; One of the purposes of a zone is to define a fire compartmentation. In this case it defines the geometric information about the fire compartment (through the contained spaces) and information, whether this compartment is ventilated or sprinkler protected. In addition the fire risk code and the hazard type can be added, the coding is normally defined within a national fire regulation. All that information is available within the relevant property sets. Again, if an independent shape has to be provided to the fire compartment, then the entity _IfcSpatialZone_ shall be used.

In case of a zone denoting a (fire) compartment, the following types should be used, if applicable, as values of the _ObjectType_ attribute:

* **'FireCompartment'**: a zone of spaces, collected to represent a single fire compartment.
* **'ElevatorShaft'**: a collection of spaces within an elevator, potentially going through many storeys.
* **'RisingDuct'**: A collection of vertical airspaces.
* **'RunningDuct'**: A collection of horizontal airspaces.