The _IfcSharedFacilitiesElements_ Schema defines basic concepts in the facilities management (FM) domain. This schema, along with _IfcProcessExtension, IfcSharedMgmtElements_and _IfcFacilitiesMgmtDomain_, provide a set of models that can be used by applications needing share information concerning facilities management related issues.

### Scope
The _IfcSharedFacilitiesElements_ schema supports ideas including:

* Furniture. 
* Grouping of elements of system furniture into individual furniture items. 
* Asset identification. 
* Inventory of objects (including asset, furniture and space objects within separate inventories).

<table cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td width="41"><a href="./lexical/text/SharedFacilitiesElements-Usage.htm"><img src="./lexical/text/img/go.gif" alt="go" border="0" height="20" width="38"></a></td>
      <td bgcolor="#c8c8c8">see attached document for more
on facilities elements</td>
    </tr>
  </tbody>
</table>

****Property Set Use Definition****:

In addition to the property sets that relate specifically to entities within this schema, the following property sets defined within this schema for support of general entities are part of this IFC release:

* [Pset_ManufacturerOccurrence](../psd/IfcSharedFacilitiesElements/Pset_ManufacturerOccurrence.xml): property set for the properties that may be given by the manufacturer of individual occurrences of manufactured products (subtypes of _IfcElement_), if available 
* [Pset_ManufacturerTypeInformation](../psd/IfcSharedFacilitiesElements/Pset_ManufacturerTypeInformation.xml): property set for the properties that may be given by the manufacturer of a type of manufactured products (subtypes of _IfcElement_ or of _IfcElementType_), if available 
* [Pset_PropertyAgreement](../psd/IfcSharedFacilitiesElements/Pset_PropertyAgreement.xml): specific property set for the properties defined within a property agreement that may be associated with an occurrence of _IfcSpatialStructureElement_ 
* [Pset_Reliability](../psd/IfcSharedFacilitiesElements/Pset_Reliability.xml): specific property set for the properties defining risk that may be associated with any occurrence of a subtype of _IfcProduct_, if available
* [Pset_Risk](../psd/IfcSharedFacilitiesElements/Pset_Risk.xml): specific property set for the properties defining risk that may be associated with any occurrence of a subtype of _IfcObject_, if available 
* [Pset_Warranty](../psd/IfcSharedFacilitiesElements/Pset_Warranty.xml): specific property set for the properties relating to a warranty or guarantee that may be associated with any occurrence of _IfcProduct_ or any occurrence of _IfcSystem_, if available
