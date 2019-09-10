A transport element is a generalization of all transport related objects that move people, animals or goods within a building or building complex. The _IfcTransportElement_ defines the occurrence of a transport element, that (if given), is expressed by the _IfcTransportElementType_.

> EXAMPLE&nbsp; Transportation elements include elevator (lift), escalator, moving walkway, etc.

> NOTE&nbsp; More detailed equipment that may be a part of a transportation device, like a lifting hook, is defined as _IfcDiscreteAccessory_. It maybe included as a part of the _IfcTransportElement_ by virtue of the objectified relationship _IfcRelAggregates_.

Depending on local classification systems transport elements and transportation systems in buildings are either considered as part of a building system, or as part of a building service system. Within IFC they are considered as part of a building system and may have to be mapped appropriately.

> HISTORY&nbsp; New entity in IFC2x.

{ .change-ifc2x}
> IFC2x CHANGE&nbsp; The attribute _PredefinedType_ (previously OperationType) is made optional.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The last attributes CapacityByWeight and CapacityByNumber are removed, use Pset_TransportElementCommon instead.
