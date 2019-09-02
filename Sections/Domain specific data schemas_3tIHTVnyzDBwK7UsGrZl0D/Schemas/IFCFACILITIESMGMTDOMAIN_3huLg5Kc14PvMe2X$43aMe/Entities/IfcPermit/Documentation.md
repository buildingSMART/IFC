An _IfcPermit_ is a document that allows permission to carry out actions in places and on artifacts where security or other access restrictions apply.

> <font color="#0000ff" size="-1">HISTORY:
New Entity in IFC 2x2</font>

****Use Definitions****

The permit will identify the restrictions that apply and when access may be gained to carry out the actions.

IfcRelAssignsToControl is used to identify related spaces, assets etc. upon which actions are permitted to take place.

****Property Set Use Definition****:

The property sets relating to an _IfcPermit_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcPermit_ are part of this IFC release:

* [Pset_Permit](../../psd/IfcFacilitiesMgmtDomain/Pset_Permit.xml): property set for the properties of a permit to do work or carry out an action, if available