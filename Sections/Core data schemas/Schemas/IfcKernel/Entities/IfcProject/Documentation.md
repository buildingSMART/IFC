The undertaking of some design, engineering, construction, or maintenance activities leading towards a product. The project establishes the context for information to be exchanged or shared, and it may represent a construction project but does not have to.

The representation context, in the case of a geometric representation context, which is referenced from the _IfcProject_, includes:

* the default units used
* the world coordinate system
* the coordinate space dimension
* the precision used within the geometric representations, and
* optionally the indication of the true north relative to the world coordinate system

> <small><font color="#0000ff">HISTORY&nbsp;
New Entity in IFC Release 1.0</font></small>

****Property Set Use Definition****:

The property sets relating to the _IfcProject_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcProject_ are part of this IFC release:

* [Pset_ProjectCommon](../../psd/IfcKernel/Pset_ProjectCommon.xml){ target="SOURCE"}: common property set for the single project occurrence.

****Spatial Structure Use Definition****

The _IfcProject_ is used to reference the root of&nbsp;the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together, and to the _IfcProject_, by using the objectified relationship _IfcRelAggregates_. The _IfcProject_ references them by its inverse relationship:

* _IfcProject.Decomposes_ -- referencing (_IfcSite_ || _IfcBuilding_) by _IfcRelAggregates.RelatingObject_. The IfcSite or IfcBuilding referenced shall be the root of the spatial structure.
* _IfcProject.IsDecomposedBy_ -- it shall be NIL, i.e. the _IfcProject_ shall not be decomposed into any parts.

**Informal propositions**:
1. There shall only be one project within the exchange context. This is enforced by the global rule _IfcSingleProjectInstance_.
