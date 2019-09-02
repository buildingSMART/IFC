This enumeration type is used to distinguish between possible action types at a high level. It can be used for an automated definition of load combinations and for dimensioning. The contained items and their acronyms are adopted from the Eurocode standard.

The _IfcActionTypeEnum_ type is referenced by the entity _IfcStructuralLoadGroup_ which shall normally be of the type LOAD_COMBINATION_GROUP (see also _IfcLoadGroupTypeEnum_). If an enumeration item is missing for an appropriate definition of a load group, the item USERDEFINED shall be used instead. In this case, a meaning can be given by using the _IfcActionSourceTypeEnum_.

> <font color="#0000FF" size="-1">HISTORY: New type in Release IFC2x
		  Edition 2. </font>
>