> NOTE&nbsp; By using the inverse relationship _IfcBuildingStorey.Decomposes_ it references (_IfcBuilding_ || _IfcBuildingStorey_) through _IfcRelAggregates.RelatingObject_IfcBuildingStorey_, the referenced 
_IfcBuildingStorey_ needs to have a different and higher
 _CompositionType_, i.e. COMPLEX (if the other _IfcBuildingStorey_ has ELEMENT), or ELEMENT (if the other
 _IfcBuildingStorey_ has PARTIAL)._