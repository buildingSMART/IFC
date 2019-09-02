An _IfcInventory_ is a list of items within an enterprise.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Modified in IFC 2x2.</font>

### Use Definitions
Various types of inventory can be included. These are identified by the range of values within the inventory type enumeration which currently includes space, asset, furniture. User defined inventories can also be defined for lists of particular types of element such as may be required in operating and maintenance instrucions. Such inventories should be constrained to contain a list of elements of a restricted type.

There are a number of actors that can be associated with an inventory, each actor having a role. Principal actors are identified as attributes of the class. Additional actors can be specified through the relationship class _IfcRelAssignsToActor_ in which case roles should be defined through the _IfcActorRole_ class which must be asserted for each defined role.

There are a number of costs that can be associated with an inventory, each cost having a role. Principal costs are identified as attributes of the class. Additional costs can be specified through the relationship class _IfcRelAssociatesCost_ in which case roles must be asserted.