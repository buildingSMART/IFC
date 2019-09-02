Generalization of all elements that participate in a distribution system. Typical examples of _IfcDistributionElement_ are (among others):

* building service elements within a heating systems 
* building service elements within a cooling system 
* building service elements within a ventilation system 
* sanitary elements 
* electrical elements 
* elements within a communication network 

The _IfcDistributionElement_ is further specialized in the IFC model. Direct instantiation of _IfcDistributionElement_ without an assigned subtype of _IfcDistributionElementType_ provides the meaning of an distribution element proxy.

> <small><font color="#0000FF">HISTORY New entity in IFC
      Release 1.5.</font></small>

****Type Use Definition****

The _IfcDistributionElement_ defines the occurrence of any HVAC, electrical, sanitary or other element within a distribution system. Common information about distribution element types (or styles) is handled by subtypes of _IfcDistributionElementType_. The _IfcDistributionElementType_ (if present) may establish the common type name, usage (or predefined) type, common material, common set of properties and common shape representations (using _IfcRepresentationMap_). The _IfcDistributionElementType_ is attached using the _IfcRelDefinedByType.RelatingType_ objectified relationship and is accessible by the inverse _IsDefinedBy_ attribute.

The assignment of types to distribution element occurrences is vital for providing the additional meaning, or ontology, of the distribution element. Many specialized type are defined in other schemas of the IFC specification.

****Quantity Use Definition****

The quantities relating to the _IfcDistributionElement_ are defined by the _IfcElementQuantity_ and attached by the _IfcRelDefinesByProperties_. A detailed specification for individual quantities is introduced at the level of subtypes of _IfcDistributionElement_.

****Geometry Use Definitions****

The geometric representation of _IfcDistributionElement_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representation.

**Local Placement**

The local placement for _IfcDistributionElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ , which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**Geometric Representations**

The geometric representation of _IfcDistributionElement_ is defined using different geometric representation types for the various subtypes. Only general recommendations are given at the level of the supertype, further constraints are defined at the level of its subtypes.

* all occurrences of _IfcDistributionElement_ (and its subtypes) should (whenever possible) share a representation map established by the assigned type. The geometric representation of the occurrence is then an _IfcMappedItem_. The _IfcShapeRepresentation_ has: 
    *  _RepresentationIdentifier_ : 'Body' 
    *  _RepresentationType_ : 'MappedRepresentation'  

The shared geometric representation of the distribution element type (or in some cases of the distribution element) should follow (if applicable) the the following guidelines:

* all fixtures (all non distribution flow elements, i.e. everything which is not a duct, a pipe, a cable, or a cable carrier) should be defined by an b-rep geometry. This includes also the complex flow fitting elements (e.g. Y branch or T branch) or distribution flow elements with size changes (e.g. reducer). The _IfcShapeRepresentation_ has: 
    *  _RepresentationIdentifier_ : 'Body' 
    *  _RepresentationType_ : 'Brep'       
* if the geometric model consistency of a b-rep shape representation can not be guaranteed (arcwise connected volume bounded by faces, each being connected, oriented, finite, closed 2-manifold), a surface representation based on open shells should be used. The _IfcShapeRepresentation_ then has: 
    *  _RepresentationIdentifier_ : 'Body' 
    *  _RepresentationType_ : 'SurfaceModel'       
* all "simple" distribution flow elements (general ducts and pipes) are defined by sweep geometry. The _IfcShapeRepresentation_ has: 
    *  _RepresentationIdentifier_ : 'Body' 
    *  _RepresentationType_ : 'SweptSolid'       
* an additional representation type for all "simple" distribution flow elements (general ducts and pipes) is the ability to have a simple line based representation. The _IfcShapeRepresentation_ has: 
    *  _RepresentationIdentifier_ : 'FootPrint' 
    *  _RepresentationType_ : 'GeometricCurveSet'       
* if only the analytical shape is required for which the exact interpolation between the cross sections is not required, a sectioned spine can be used. 
    *  _RepresentationIdentifier_ : 'Body' 
    *  _RepresentationType_ : 'SectionedSpine'