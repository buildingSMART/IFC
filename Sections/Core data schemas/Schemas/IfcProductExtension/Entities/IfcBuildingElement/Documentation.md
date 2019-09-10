The building element comprises all elements that are primarily part of the construction of a building, i.e., its structural and space separating system.

{ .extDef}
> "Major functional part of a building, examples are foundation, floor, roof, wall." ISO 6707-1

> EXAMPLE&nbsp; Building elements are walls, beams, or doors, they are all physically existent and tangible things.

The _IfcBuildingElement_ utilizes the following capabilities mainly through inverse attributes referencing objectified relationships:

> NOTE&nbsp; View definitions and implementer agreements will determine those relationships that have to be supported in actual exchange.

1. Grouping - being part of a logical group of objects 
    * objectified relationship: _IfcRelAssignsToGroup_
    * object referenced by relationship: _IfcGroup_ (and subtypes)
    * inverse attribute: _HasAssignment_ 
2. Work processes - reference to work tasks, in which this building element is used 
    * objectified relationship: _IfcRelAssignsToProcess_
    * object referenced by relationship: _IfcProcess_ (and subtypes)
    * inverse attribute: _HasAssignments_ 
3. Structural member reference - information whether the building element is represented in a structural analysis model by a structural member 
    * objectified relationship: _IfcRelAssignsToProduct_
    * object referenced by relationship: _IfcStructuralMember_ (and by default _IfcStructuralCurveMember_)
    * inverse attribute: _HasAssignments_ 
4. Aggregation - aggregated together with other elements to form an aggregate 
    * objectified relationship: _IfcRelAggregates_
    * object referenced by relationship: _IfcElement_ (and subtypes)
    * inverse attribute (for container): _IsDecomposedBy_
    * inverse attribute (for contained parts): _Decomposes_ 
5. Material - assignment of material used by this building element 
    * objectified relationship: _IfcRelAssociatesMaterial_
    * object referenced by relationship: _IfcMaterialSelect_ (and selected items)
    * inverse attribute: _HasAssociations_ 
6. Classification - assigned reference to an external classification 
    * objectified relationship: _IfcRelAssociatesClassification_
    * object referenced by relationship: _IfcClassificationNotationSelect_ (and selected items, default _IfcClassificationReference_)
    * inverse attribute: _HasAssociations_ 
7. Library - assigned reference to an external library item reference 
    * objectified relationship: _IfcRelAssociatesClassification_
    * object referenced by relationship: _IfcLibrarySelect_ (and selected items, default _IfcLibraryReference_)
    * inverse attribute: _HasAssociations_ 
8. Documentation - assigned reference to an external documentation 
    * objectified relationship: _IfcRelAssociatesDocumentation_
    * object referenced by relationship: _IfcDocumentSelect_ (and selected items, default _IfcDocumentReference_)
    * inverse attribute: _HasAssociations_ 
9. Type - reference to the common product type information for the element occurrence 
    * objectified relationship: _IfcRelDefinesByType_
    * object referenced by relationship: _IfcBuildingElementType_ (and subtypes)
    * inverse attribute: <font color="#0000FF"><em>IsTypedBy</em></font> 
10. Properties - reference to all attached properties, including quantities 
    * objectified relationship: _IfcRelDefinesByProperties_
    * object referenced by relationship: _IfcPropertySetDefinition_ (default _IfcPropertySet_)
    * inverse attribute: _IsDefinedBy_ 
11. Connection - connectivity to other elements, including the definition of the joint 
    * objectified relationship: _IfcRelConnectsElements_
    * object referenced by relationship: _IfcElement_
    * inverse attribute: _ConnectedTo_
    * inverse attribute: _ConnectedFrom_ 
12. Realization - information, whether the building element is used to realize a connection (e.g. as a weld in a connection between two members) 
    * objectified relationship: _IfcRelConnectsWithRealizingElements_
    * object referenced by relationship: _IfcElement_
    * inverse attribute: _IsConnectionRealization_ 
13. Assignment to spatial structure - hierarchical assignment to the right level within the spatial structure 
    * objectified relationship: _IfcRelContainedInSpatialStructure_
    * object referenced by relationship: _IfcSpatialStructureElement_
    * inverse attribute: _ContainedInStructure_ 
14. Reference to spatial structure(s) - non hierarchical reference to one or more elements within the spatial structure (e.g. a curtain wall, being contained in the building, references several stories) 
    * objectified relationship: _IfcRelReferencedInSpatialStructure_
    * object referenced by relationship: _IfcSpatialElement_
    * inverse attribute: _ReferencedInStructure_ 
15. Boundary - provision of space boundaries by this building element 
    * objectified relationship: _IfcRelSpaceBoundary_
    * object referenced by relationship: _IfcSpace_
    * inverse attribute: _ProvidesBoundaries_ 
16. Coverings - assignment of covering elements to this building element (note: normally covering elements are assigned to the space, only used for special cases) 
    * objectified relationship: _IfcRelCoversBldgElements_
    * object referenced by relationship: _IfcCovering_
    * inverse attribute: _HasCoverings_ 
17. Voids - information, whether the building element includes openings, recesses or other voids 
    * objectified relationship: _IfcRelVoidsElement_
    * object referenced by relationship: _IfcFeatureElementSubtraction_ (default _IfcOpeningElement_)
    * inverse attribute: _HasOpenings_ 
18. Projection - information, whether the building element has projections (such as a fascia) 
    * objectified relationship: _IfcRelProjectsElement_
    * object referenced by relationship: _IfcFeatureElementAddition_ (default _IfcProjectionElement_)
    * inverse attribute: _HasProjections_ 
19. Filling - information whether the building element is used to fill openings 
    * objectified relationship: _IfcRelFillsElement_
    * object referenced by relationship: _IfcOpeningElement_
    * inverse attribute: _FillsVoids_ 

> HISTORY&nbsp; New entity in IFC1.0

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)
* _IfcElement_: [Product Placement](../../templates/product-placement.htm), [Box Geometry](../../templates/box-geometry.htm), [FootPrint Geometry](../../templates/footprint-geometry.htm), [Body SurfaceOrSolidModel Geometry](../../templates/body-surfaceorsolidmodel-geometry.htm), [Body SurfaceModel Geometry](../../templates/body-surfacemodel-geometry.htm), [Body Tessellation Geometry](../../templates/body-tessellation-geometry.htm), [Body Brep Geometry](../../templates/body-brep-geometry.htm), [Body AdvancedBrep Geometry](../../templates/body-advancedbrep-geometry.htm), [Body CSG Geometry](../../templates/body-csg-geometry.htm), [Mapped Geometry](../../templates/mapped-geometry.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcbuildingelement.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_ConcreteElementGeneral.xml">Pset_ConcreteElementGeneral</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementFabrication.xml">Pset_PrecastConcreteElementFabrication</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcstructuralelementsdomain/Pset_PrecastConcreteElementGeneral.xml">Pset_PrecastConcreteElementGeneral</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Condition.xml">Pset_Condition</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactIndicators.xml">Pset_EnvironmentalImpactIndicators</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcproductextension/Pset_EnvironmentalImpactValues.xml">Pset_EnvironmentalImpactValues</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerOccurrence.xml">Pset_ManufacturerOccurrence</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ManufacturerTypeInformation.xml">Pset_ManufacturerTypeInformation</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedmgmtelements/Pset_PackingInstructions.xml">Pset_PackingInstructions</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_ServiceLife.xml">Pset_ServiceLife</a></td></tr>
<tr><td>&nbsp;</td><td><a href="../../psd/ifcsharedfacilitieselements/Pset_Warranty.xml">Pset_Warranty</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcBuildingElement Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Product Assignment

The [Product Assignment](../../templates/product-assignment.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Type</b></th><th><b>Description</b></th></tr>
<tr><td><a href="../../ifcprocessextension/lexical/ifctask.htm">IfcTask</a></td><td>Task for operating upon the building element.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcBuildingElement Product Assignment</p></td></tr></table>

  
  
{ .use-head}
Spatial Containment

The [Spatial Containment](../../templates/spatial-containment.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Structure</b></th></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuildingstorey.htm">IfcBuildingStorey</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcbuilding.htm">IfcBuilding</a></td></tr>
<tr><td><a href="../../ifcproductextension/lexical/ifcsite.htm">IfcSite</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcBuildingElement Spatial Containment</p></td></tr></table>

  
  
{ .use-head}
Surface 3D Geometry

The [Surface 3D Geometry](../../templates/surface-3d-geometry.htm) concept applies to this entity.

Some _IfcBuildingElement_ may be represented by an surface as an abstract geometric representation. See each subtype for specific guidance.