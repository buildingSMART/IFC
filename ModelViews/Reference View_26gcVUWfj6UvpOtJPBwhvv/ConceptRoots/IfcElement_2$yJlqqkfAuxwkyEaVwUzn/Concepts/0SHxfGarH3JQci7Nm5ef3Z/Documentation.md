Placement of elements is defined by a local placement (a transformation matrix relative to):

* the spatial container (if not part of an assembly) 
    * provided by the relationship _IfcRelContainedInSpatialStructure_._RelatingSpatialStructure_
    * being a subtype of _IfcSpatialElement_, in most cases, _IfcBuildingStorey_ 
* the parent aggregation element (if it is an aggregated part) 
    * provided by the relationship _IfcRelAggregates_._RelatingObject_
    * being a subtype of _IfcElement_ 

The local placement shall always be relative.