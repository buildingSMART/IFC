This type definition is used to distinguish between different kinds and purposes of load grouping. It allows to differentiate between load groups, load cases, load combination groups and load combinations. Normally, these enumeration types shall be used in the following context :

* LOAD_GROUP groups instances of _IfcStructuralAction_ or its subclasses. It shall be used as a container for loads grouped together for specific purposes. Optionally, an overall load factor can be assigned. 
* LOAD_CASE groups LOAD_GROUPs and instances of _IfcStructuralAction_ or its subclasses. It shall be used as a container for loads with the same origin, and to assign a common load factor. 
* LOAD_COMBINATION_GROUP shall be used to group LOAD_CASEs and to assign a common load combination factor. The grouping of LOAD_GROUPs and instances of _IfcStructuralAction_ or its subclasses is also possible, but off the traditional way. 
* LOAD_COMBINATION shall be used to group all loads belonging to a specific load combination. Normally only LOAD_COMBINATION_GROUPs with all needed load factors are used to create load combinations. 

The _IfcLoadGroupTypeEnum_ type is referenced by the entity _IfcStructuralLoadGroup_.

> <font color="#0000FF" size="-1">HISTORY: New type in Release IFC2x
		  Edition 2. </font>
>