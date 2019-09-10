The element type _IfcDistributionControlElementType_ defines a list of commonly shared property set definitions of an element and an optional set of product representations. It is used to define an element specification (the specific product information that is common to all occurrences of that product type).

Distribution control element types (or the instantiable subtypes) may be exchanged without being already assigned to occurrences.

The occurrences of the _IfcDistributionControlElementType_ are represented by instances of _IfcDistributionControlElement_ or its subtypes.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Ports may now be defined using _IfcRelNests_ to enable definition of ports at type definitions (both forward and backward compatible), provide a logical order, and reduce the number of relationship objects needed. The relationship _IfcRelConnectsPortToElement_ is still supported on occurrence objects, however is now specific to dynamically connected ports.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcdistributioncontrolelementtype.htm)

{ .use-head}
Product Type Assignment

The [Product Type Assignment](../../templates/product-type-assignment.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifctasktype.htm">IfcTaskType</a></td><td>Indicates task types available to purchase, install, renovate, demolish, operate, or otherwise act upon occurrences of the element type.  Such task types may be instantiated as task occurrences assigned to occurrences of the element type.  Prices (such as for purchasing or shipping) may be established by resource types assigned to task types.</td></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifcproceduretype.htm">IfcProcedureType</a></td><td>Indicates procedure types available to operate occurrences of the element type.  Such procedure types may be instantiated as procedure occurrences assigned to occurrences of the element type.</td></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifceventtype.htm">IfcEventType</a></td><td>Indicates event types available to be raised by occurrences of the element type, sequenced by procedures to be followed.  Such event types may be instantiated as event occurrences assigned to occurrences of the element type.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcDistributionControlElementType Product Type Assignment</p></td></tr></table>