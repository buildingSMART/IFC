## Introduction
The _IfcFacilitiesMgmtDomain_ Schema defines basic concepts in the facilities management (FM) domain. Together with the _IfcProcessExtension_, _IfcSharedMgmtElements_, and _IfcSharedFacilitiesElements_ schema, it provides a set of models that can be used to exchange information between facilities management applications.

## Scope
The _IfcFacilitiesMgmtDomain_ schema forms part of the Domain Layer of the IFC Model. It extends the ideas concerning facilities management outlined in the _IfcSharedFacilitiesElements_ schema and management in general outlined in the _IfcSharedMgmtElements_ schema. The objective is to capture information that supports specific business processes that are wholly within the domain of interest of the Facilities Manager. The aim is to provide support for information exchange and sharing within computer aided facilities management and computer aided maintenance management applications. The extent of the model will not support the some of the more detailed ideas found in these applications.

The following are within the scope of this part of the specifications:

*  Managing the movement of people and their associated equipment from one place to another. All types of move are considered to be within scope ranging from moving a single person from one office to another to the movement of complete organizations between locations.
*  The assignment of facilities management standards according to roles played by actors within an organization. Assignment of standards is limited to space, furniture and equipment.
* Capturing information concerning the condition of components and assets both for subjective and objective assessment of condition.
*  Recording the assignment of permits for access and carrying out work.
*  Capturing requests for action to be carried out and the assignment of work orders to fulfill the needs expressed by requests.

The following are outside of the scope of this part of the specifications:

*  Work interactions between actors and between space programs.
* Moving or identifying the movement of or identifying the need for (as a result of moving) electrical or telecommunications services or connection points or the need for new electrical or telecommunications equipment as a result of the move.
* Facilities management standards other than space, furniture and equipment.

<table cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td width="41"><a href="lexical/text/IfcFacilitiesMgmtDomain_Usage.htm" target="SOURCE"><img src="lexical/text/img/go.gif" alt="go" border="0" height="20" width="38"></a></td>
      <td bgcolor="#c8c8c8">see attached document for more
on facilities management usage</td>
    </tr>
  </tbody>
</table>

****Property Set Use Definition****:

In addition to the property sets that relate specifically to entities within this schema, the following property sets defined within this schema for support of general entities are part of this IFC release:

* [Pset_PackingInstructions](../psd/IfcFacilitiesMgmtDomain/Pset_PackingInstructions.xml): property set for the properties that may be given by the manufacturer of of manufactured products (subtypes of _IfcElement_) concerning their packing/packaging, if available