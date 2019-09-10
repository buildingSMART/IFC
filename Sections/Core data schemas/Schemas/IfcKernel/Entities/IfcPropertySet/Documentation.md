The _IfcPropertySet_ defines all dynamically extensible properties. The property set is a container class that holds properties within a property tree. These properties are interpreted according to their name attribute.

Property sets, defining a particular type of object, can be assigned an object type (_IfcTypeObject_). Property sets are assigned to objects (_IfcObject_) through an objectified relationship (_IfcRelDefinedByProperties_). If the same set of properties applies to more than one object, it should be assigned by a single instance of _IfcRelDefinedByProperties_ to a set of related objects. Those property sets are referred to as shared property sets.

> <small><font color="#0000ff">HISTORY&nbsp;
New Entity in IFC Release 1.0
  </font></small>

**Use Definition**

Instances of _IfcPropertySet_ are used to assign named sets of individual properties (complex or single properties). Each individual property has a significant name string. Some property sets have&nbsp;predefined instructions on assigning those significant name, these are listed under "property sets" main menu item within this specification. The naming convention "Pset_Xxx" applies to those property sets and shall be used as the value to the _Name_ attribute.

In addition any user defined property set can be captured, those property sets shall have a _Name_ value not including the "Pset_" prefix.
