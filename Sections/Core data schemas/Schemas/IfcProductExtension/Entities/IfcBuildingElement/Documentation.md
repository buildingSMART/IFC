**Definition from ISO 6707-1:1989**: Major functional part of a building, examples are foundation, floor, roof, wall.

The building element comprises all elements that are primarily part of the construction of a building, i.e., its structural and space separating system.

> <small>EXAMPLEs of building elements are walls, beams, or
      doors, they are all physically existent and tangible
      things.</small>

The _IfcBuildingElement_ utilizes the following capabilities mainly through inverse attributes referencing objectified relationships:

1. Grouping - being part of a logical group of objects 
    * objectified relationship: _IfcRelAssignsToGroup_ 
    * inverse attribute: _HasAssignment_ 
2. Work processes - reference to work tasks, in which this building element is used 
    * objectified relationship: _IfcRelAssignsToProcess_ 
    * inverse attribute: _HasAssignments_ 
3. Aggregation - aggregated together with other elements to form an aggregate 
    * objectified relationship: _IfcRelAggregates_ 
    * inverse attribute (for container): _IsDecomposedBy_ 
    * inverse attribute (for contained parts): _Decomposes_ 
4. Material - assignment of material used by this building element 
    * objectified relationship: _IfcRelAssociatesMaterial_ 
    * inverse attribute: _HasAssociations_ 
5. Classification - assigned reference to an external classification 
    * objectified relationship: _IfcRelAssociatesClassification_ 
    * inverse attribute: _HasAssociations_ 
6. Documentation - assigned reference to an external documentation 
    * objectified relationship: _IfcRelAssociatesDocumentation_ 
    * inverse attribute: _HasAssociations_ 
7. Type - reference to the common product type information for the element occurrence 
    * objectified relationship: _IfcRelDefinesByType_ 
    * inverse attribute: _IsDefinedBy_ 
8. Properties - reference to all attached properties, including quantities 
    * objectified relationship: _IfcRelDefinesByProperties_ 
    * inverse attribute: _IsDefinedBy_ 
9. Connection - connectivity to other elements, including the definition of the joint 
    * objectified relationship: _IfcRelConnectsElements_ 
    * inverse attribute: _ConnectedTo_ 
    * inverse attribute: _ConnectedFrom_ 
10. Realization - information, whether the building element is used to realize a connection (e.g. as a weld in a connection between two members) 
    * objectified relationship: _IfcRelConnectsWithRealizingElements_ 
    * inverse attribute: _IsConnectionRealization_ 
11. Ports - information, whether the building element has ports for system connections (note: normally not used, this relationship is inherited from _IfcElement_ and mainly applicable to _IfcDistributionElement_'s) 
    * objectified relationship: _IfcRelConnectsPortToElement_ 
    * inverse attribute: _HasPorts_ 
12. Assignment to spatial structure - hierarchical assignment to the right level within the spatial structure 
    * objectified relationship: _IfcRelContainedInSpatialStructure_ 
    * inverse attribute: _ContainedInStructure_ 
13. Reference to spatial structure(s) - non hierarchical reference to one or more elements within the spatial structure (e.g. a curtain wall, being contained in the building, references several stories) 
    * objectified relationship: _IfcRelContainedInSpatialStructure_ 
    * inverse attribute: _ContainedInStructure_ 
14. Boundary - provision of space boundaries by this building element 
    * objectified relationship: _IfcRelSpaceBoundary_ 
    * inverse attribute: _ProvidesBoundaries_ 
15. Coverings - assignment of covering elements to this building element (note: normally covering elements are assigned to the space, only used for special cases) 
    * objectified relationship: _IfcRelCoversBldgElements_ 
    * inverse attribute: _HasCoverings_ 
16. Voids - information, whether the building element includes openings, recesses or other voids 
    * objectified relationship: _IfcRelVoidsElement_ 
    * inverse attribute: _HasOpenings_ 
17. Projection - information, whether the building element has projections (such as a fascia) 
    * objectified relationship: _IfcRelProjectsElement_ 
    * inverse attribute: _HasProjections_ 
18. Filling - information whether the building element is used to fill openings 
    * objectified relationship: _IfcRelFillsElement_ 
    * inverse attribute: _FillsVoids_ 
19. Structural member reference - information whether the building element is represented in a structural analysis model by a structural member 
    * objectified relationship: _IfcRelConnectsStructuralElement_ 
    * inverse attribute: _HasStructuralMember_ 

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
        Release 1.0</font>
> 


****Quantity Use Definition****:

The quantities relating to the _IfcBuildingElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. A detailed specification for individual quantities is introduced at the level of subtypes of _IfcBuildingElement_.

****Geometry Use Definitions****

The geometric representation of any _IfcBuildingElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local Placement**

The local placement for any _IfcBuildingElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations. Further constraints are defined at the level of its subtypes.

**_Geometric Representations_**

Any _IfcBuildingElement_ can be represented by one or several geometric representations. A detailed specification is introduced at the level of subtypes. Only the general representation types 'BoundingBox', 'SurfaceModel', 'Brep', and 'MappedRepresentation' are defined here.

**Bounding Box Representation**

Any _IfcBuildingElement_ may be represented as a bounding box, which shows the maximum extend of the body within the coordinated system established by the _IfcLocalPlacement_. The bounding box representation is the simplest geometric representation available. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Box' ~~Body~~ 
*  _RepresentationType_ : 'BoundingBox' 

<table>
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcBuildingElement-BoundingBox-Layout1.dwf">
            <img src="figures/ifcbuildingelement-boundingbox-layout1.gif" alt="bounding box" border="0" height="275" width="400"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The bounding box representation is
              given by an <i>IfcShapeRepresentation</i>, which
              includes a single item, an
              <i>IfcBoundingBox</i>.</font>
            </p>
          </td>
        </tr>
      </tbody>
    </table>

**SurfaceModel Representation**

Any _IfcBuildingElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple surface models, based on either shell or face based models. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'SurfaceModel' 

In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

<table>
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcBuildingElement-SurfaceModel-Layout1.dwf">
            <img src="figures/ifcbuildingelement-surfacemodel-layout1.gif" alt="bounding box" border="0" height="275" width="400"></a>
          </td>
          <td align="left" valign="top">
            <p>
              <font size="-1">The surface model representation is
              given by an IfcShapeRepresentation, which includes
              a single item, which is either:</font>
            </p>
            <ul>
              <li>
                <font size="-1"><i>IfcShellBasedSurfaceModel</i>,
                or</font>
              </li>
              <li>
                <font size="-1"><i>IfcFaceBasedSurfaceModel</i>.</font>
              </li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>

**Brep Representation**

Any _IfcBuildingElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation elements (which are restricted to faceted Brep with or without voids). The Brep representation allows for the representation of complex element shape. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'Brep' 

In some cases it may be useful to also expose a simple representation as a bounding box representation of the same complex shape.

<table cellpadding="2" cellspacing="2">
      <tbody>
        <tr valign="top">
          <td align="left" valign="top">
            <a href="drawings/IfcBuildingElement-BRep-Layout1.dwf"><img src="figures/ifcbuildingelement-brep-layout1.gif" alt="Brep representation" border="0" height="275" width="400"></a>
          </td>
          <td align="left" valign="top">
            TheBrep representation is given by an
            IfcShapeRepresentation, which includes one or more
            items, all of type IfcManifoldSolidBrep.
          </td>
        </tr>
      </tbody>
    </table>

**MappedRepresentation**

Any _IfcBuildingElement_ (so far no further constraints are defined at the level of its subtypes) may be represented using the MappedRepresentation. This shall be supported as it allows for reusing the geometry definition of a type at all occurrences of the same type. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

*  _RepresentationIdentifier_ : 'Body' 
*  _RepresentationType_ : 'MappedRepresentation' 

The same constraints, as given for the 'SurfaceModel' and the 'Brep' geometric representation, shall apply to the _MappedRepresentation_ of the _IfcRepresentationMap_.
