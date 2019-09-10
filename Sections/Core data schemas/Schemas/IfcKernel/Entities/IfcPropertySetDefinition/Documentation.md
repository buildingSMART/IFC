An _IfcPropertySetDefinition_ is a generalization of property sets, that are either:

> **Dynamically extendable properties**, they define properties for which the IFC model only provides a kind of "meta model", to be further declared by agreement. This means no entity definition of the properties exists within the IFC model. The declaration is done by assigning a significant string value to the&nbsp;_Name_ attribute of the entity as defined in the entity _IfcPropertySet_ and at each subtype of _IfcProperty_, referenced by the property set.
> 
> **Statically defined properties**, they define properties for which an entity definition exists within the IFC model. The semantic meaning of each statically defined property is declared by its entity type and the meaning of the properties is defined by the name of the explicit attribute.
> 


The subtypes of the _IfcPropertySetDefinition_ are either the dynamically extendable _IfcPropertySet_, or all other statically defined subtypes.

> <small><font color="#0000ff">HISTORY&nbsp;
New Entity in IFC Release 2x
  </font></small>
