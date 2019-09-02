The _IfcActor_ defines all actors or human agents involved in a project during its full life cycle. It facilitates the use of person and organization definitions in the resource part of the IFC object model. This includes name, address, telecommunication addresses, and roles.

> HISTORY&nbsp; New entity in IFC2.0

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcactor.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifckernel/Pset_ActorCommon.xml">Pset_ActorCommon</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcActor Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Actor Assignment

The [Actor Assignment](../../templates/actor-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifckernel/lexical/ifccontrol.htm">IfcControl</a></td><td>Indicates project directives issued by the actor.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcgroup.htm">IfcGroup</a></td><td>Indicates groups for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcproduct.htm">IfcProduct</a></td><td>Indicates products for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcprocess.htm">IfcProcess</a></td><td>Indicates processes for which the actor is responsible.</td></tr>
<tr><td><a href="../../ifckernel/lexical/ifcresource.htm">IfcResource</a></td><td>Indicates resources for which the actor is responsible.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcActor Actor Assignment</p></td></tr></table>