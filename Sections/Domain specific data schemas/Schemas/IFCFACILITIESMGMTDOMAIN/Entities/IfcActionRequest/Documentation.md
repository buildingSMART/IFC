An _IfcActionRequest_ is a request for an action to fulfill a need.

> <font color="#0000ff" size="-1">HISTORY:
New Entity in IFC 2x2</font>

****Use Definitions****

Requests may take many forms depending on the need including fault reports for maintenance, requests for small works, purchase requests (where these are to be made through a help desk or buying function) etc.

A request may call for several actions and an action may refer to several requests. _IfcRelAssignsToControl_ is used to relate one or more requests to an action.

****Property Set Use Definition****:

The property sets relating to an _IfcActionRequest_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcActionRequest_ are part of this IFC release:

* [Pset_ActionRequest](../../psd/IfcFacilitiesMgmtDomain/Pset_ActionRequest.xml): property set for the properties of a request for a facilities management action, if available